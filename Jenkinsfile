pipeline {
    agent any
    
    tools {
         maven 'Default'
      }
    
    stages {
        stage('---clean---') {
            steps {
                sh "mvn clean"
                echo "clean"
            }
        }
        stage('--test--') {
            steps {
                sh "mvn test"
            }
        }
        stage('--package--') {
            steps {
                sh "mvn package"
            }
        }
    }
}
