pipeline {
    agent {label 'java_11'}
    stages{
        stage ('clone'){
            steps{
                git branch: 'main',url:'https://github.com/vamsibakka/js-e2e-express-server.git'
            }
        }
        stage ('build'){
            steps{
                sh 'npm install'
                sh 'npm build'
            }
        }
    }
}