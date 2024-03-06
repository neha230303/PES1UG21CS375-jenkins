pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ main.cpp -o temp'
                 build job: 'PES1UG21CS375-1', wait: false
                 echo 'Build by CS375 successful'
            }
        }

        stage('Test') {
            steps {
                sh 'cat main.cpp'
                echo 'Test by CS375 successful'
            }
        }

        stage('Deploy') {
            steps {
               
                 echo 'Deploy by CS375 successful'
            }
        }
    }

    post {
        failure {
            
                echo 'Pipeline Failed'
          
        }
    }
}