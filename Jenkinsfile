pipeline {
    agent any
    stages {
        stage("Clean Up"){
            steps {
                deleteDir()
            }
        }
        stage("Build"){
            steps {
                dir("Jenkins-Course"){
                    bat "npm install"
                }
            }
        }
        stage("Test"){
            steps {
              dir("Jenkins-Course"){
                    bat "npm run test"
                }  
            }
        }
    }
}
