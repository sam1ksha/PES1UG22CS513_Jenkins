pipeline {
    agent any 

    stages {
        stage('Build') {
            steps {
                script {
                    sh 'g++ main.cpp -o PES1UG22CS513-1'
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    sh './PES1UG22CS513-1'
                }
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deployment stage (Placeholder - Add actual deployment steps here)'
            }
        }
    }

    post {
        failure {
            echo 'Pipeline Failed'
        }
    }
}
