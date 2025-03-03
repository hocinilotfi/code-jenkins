pipeline{
    agent {
        docker {
            image "postman/newman"
        }
        
    }

    stages{
        stage('Test API'){
            steps{
                sh 'newman run collections/collection1.json'
            }
        }
    }
}