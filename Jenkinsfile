pipeline {
    agent any

    stages {
        stage('Dev') {
            steps {
                echo 'Deploying to Dev Environment'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the Application'
            }
        }

        stage('Test') {
            steps {
                echo 'Deploying to Application to Test Environment'
            }
        }
    }
        post {
            always {
                emailext body: 'Summary!', subject: 'Build Pipeline Status!', to: 'viveksanganna79@gmail.com'
                  }
        
         }
        
      
}
