    pipeline {
        agent any
     
        tools {
            maven 'localMaven'
        }
     
    stages{
            stage('Build'){
                steps {
                    build job: 'udemy_package_step'
                }
            }
        }
    }
