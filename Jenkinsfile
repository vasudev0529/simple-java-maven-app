pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo "Building stage"
                        
                    }
        }
        stage('Test') { 
            steps {
                sh 'mvn test' 
            }
            post {
                always {
                    junit 'target/surefire-reports/*.xml' 
                }
            }
        }
    }
}

