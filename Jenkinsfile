pipeline {
    agent any
      tools {
             maven 'MAVEN_HOME'
        }
    stages {
        stage('---clean---') {
            steps {
                sh "mvn clean compile"
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
