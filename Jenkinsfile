pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    sh 'g++ -o PES2UG22CS607-1 program.cpp' // Compile C++ file
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    sh './PES2UG22CS607-1' // Run compiled executable
                }
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
               
            }
        }
    }

    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}
