pipeline {
    agent any

    stages {

        
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
