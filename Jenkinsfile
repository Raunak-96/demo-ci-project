pipeline {
    agent any

    stages {

        stage('Read File') {
            steps {
                script {
                    def content = readFile 'raunak.txt'
                    echo content
                }
            }
        }

    }
}