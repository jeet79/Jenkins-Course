pipeline {
    agent any
    stages {
        stage("Clean Up"){
            steps {
                deleteDir()
            }
        }
        stage('Checkout Code') {
    steps {
        checkout scm
    }
}
        stage("Build"){
            steps {
                    bat "npm install"
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
