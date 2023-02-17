pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ temp.cpp -o hello'
                 build job: 'PES1UG20CS544-1', wait: false
                 echo 'Build by PES1UG20CS544 successful'
            }
        }

        stage('Test') {
            steps {
                sh 'cat hello.cpp'
                echo 'Test by PES1UG20CS544 successful'
            }
        }

        stage('Deploy') {
            steps {
               
                echo 'Deploy by PES1UG20CS544 successful'
            }
        }
    }

    post {
        failure {
            
                echo 'Pipeline Failed'
          
        }
    }
}
