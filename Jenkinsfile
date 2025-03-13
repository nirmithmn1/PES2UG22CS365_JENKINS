pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    sh 'g++ hello.cpp -o hello'
                }
            }
        }
        
        stage('Test') {
            steps {pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                sh 'g++-wrong -o PES2UG22CS365-1 PES2UG22CS365-1.cpp'
                echo 'Build Stage Successful'
            }
        }
        
        stage('Test') {
            steps {
                sh './PES2UG22CS365-1'
                echo 'Test Stage Successful'
            }
        }
        
        stage('Deploy') {
            steps {
                sh 'echo Deploying the application'
                echo 'Deployment Successful'
            }
        }
    }
    
    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}
                script {
                    sh './hello'
                }
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying Application...'
            }
        }
    }

    post {
        failure {
            echo 'Pipeline Failed'
        }
    }
}
