pipeline {
    agent any

    stages {
        stage('Restore dependencies') {
            steps {
                bat 'dotnet restore'
            }
        }

        stage('Build the project') {
            steps {
                bat 'dotnet build --no-restore'
            }
        }

        stage('Run Tests') {
            steps {
                bat 'dotnet test'
            }
        }
    }
}
