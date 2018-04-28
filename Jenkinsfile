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
            }
        }
    }
