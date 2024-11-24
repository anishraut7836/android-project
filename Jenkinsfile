pipeline {
    agent any
    options {
        // Timeout counter starts AFTER agent is allocated
        timeout(time: 1, unit: 'SECONDS')
    }
    stages {
        stage('Example') {
            steps {
                echo 'Hello World'
            }
        }
        stage('list-directory') {
            steps {
                sh '''
                ls -l
                cat test-file1

                '''
            }
        }
    }
}
