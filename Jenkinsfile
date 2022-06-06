pipeline {
    agent {openjdk11} 

    stages {
        stage('Build') {
            
            steps {
                container('jdk11') {
                echo 'Building..'
            }
            }
        }
        stage('Test') {
            steps {
                container('jdk11') {
                    echo 'Testing..'}
            }
        }
       
    }
}
