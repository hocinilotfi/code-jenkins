pipeline{
    agent {
        docker {
            image "postman/newman"
            args "--entrypoint=''"
        }
        
    }

    stages{
        stage('verifier la version de newman'){
            steps{
                sh 'newman --version'
            }
        }
        stage('Test API'){
            steps{
                sh 'newman run collections/collection1.json'
            }
        }
    }
}