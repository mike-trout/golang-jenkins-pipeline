pipeline {
    agent { docker { image 'golang:alpine' } }
    stages {
        stage('build') {
            steps {
                sh 'go version'
            }
        }
        stage('test') {
            steps {
                sh 'echo "Hello World"'
                sh '''
                    echo "Multiline shell steps works too"
                    ls -lah
                '''
            }
        }
    }
}
