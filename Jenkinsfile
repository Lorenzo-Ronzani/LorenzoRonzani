pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh '''
                    cd Assessment2
                    npm install
                    npm run build
                '''
            }
        }

        stage('Test') {
            steps {
                sh '''
                    cd Assessment2
                    npm test
                '''
            }
        }
    }
}