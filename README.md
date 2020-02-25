pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                 echo "your code"
                sh '''
                    echo "Multiline shell steps works too"
                    ls -lah
                '''
            }
        }
    }
}
