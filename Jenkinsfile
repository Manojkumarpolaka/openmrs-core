pipeline {
    agent any
    stages { 
        stage('SCM Checkout') {
            steps{
            git url: 'https://github.com/openmrs/openmrs-core.git', branch: "master"
            }
        }

        stage('Build package') {
            steps{
                sh 'mvn clean package'
            }
        }       
    }
}
