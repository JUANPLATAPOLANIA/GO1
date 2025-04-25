pipeline {
    agent { label 'agent5' }

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/JorgeAAV2005/PruebasGo.git'
            }
        }
        stage('Test') {
            steps {
                sh 'go test ./... -v -json > result.json'
            }
        }
    }


}
