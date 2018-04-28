    pipeline {
        agent any
     
        tools {
            maven 'localMaven'
        }
     
    stages{
            stage('Build'){
                steps {
                    build job: 'udemy_pipeline_package_step'
                }
                post {
                    success {
                        echo "Archiving"
                        archiveArtifacts artifacts: '**/target/*.war'
                    }
                }
            }
            stage('Deploy to Staging'){
                steps {
                    build job: 'udemy_deploy_to_staging'
                }
            }
        }
    }
