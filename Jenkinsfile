pipeline {
    agent {label 'openjdk11'} 

    stages {
        stage('clean') {
            
            steps {
                container('jdk11') {
               sh 'mvn clean'
            }
            }
        }
        stage('compile') {
            steps {
                container('jdk11') {
                    sh 'mvn compiler:compile'
                }
            }
        }
        stage('package') {
            steps {
                container('jdk11') {
                    sh 'mvn package'
                }
            }
        }
    }
}
