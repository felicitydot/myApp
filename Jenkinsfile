pipeline {
    agent any

    stages {
            
        stage('Checkout') {
            steps {
                git credentialsId: 'felicitydot' , url : 'https://github.com/felicitydot/myApp.git', branch : 'main'
            }
        }
        
        stage('Clean') {
            steps {
                bat "dotnet clean"
            }
        }
        
        stage('Build') {
            steps {
                bat "dotnet build --configuration Release"
            }
        }
        
        
    }
}
