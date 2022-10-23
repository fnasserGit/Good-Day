pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
    post{
        
        always{
            
            emailtext body: 'Summary', Subject: 'Pipeline Status', to: 'fadnasser@outlook.com'
            
        }
    }
}
