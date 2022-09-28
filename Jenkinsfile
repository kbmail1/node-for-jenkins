pipeline {
    agent { docker { image 'node:16.13.1-alpine' } }
    stages {
        stage('build') {
            steps {
                node ./hello.js
                sh 'node --version'
                sh 'echo "Hello World"'
                sh '''
                    echo "multi-line"
                    ls -lah
                '''
            }
        }
    }
}