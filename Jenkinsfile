pipeline {
    agent { label 'agent5' }

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/JUANPLATAPOLANIA/GO1.git'
            }
        }
        stage('Test') {
            steps {
                sh 'go test ./... -v -json > result.json'
            }
        }
    }


}
