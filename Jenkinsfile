pipeline {
    agent any

    stages {
        stage('Dotnet restore') {
            steps {
                bat 'dotnet restore'
            }
        }

        stage('Dotnet build') {
            steps {
                bat 'dotnet build --no-restore'
            }
        }

        stage('Dotnet test Project 1') {
            steps {
                bat 'dotnet test TestProject1/TestProject1.csproj --no-build --verbosity normal'
            }
        }
        stage('Dotnet test Project 2') {
            steps {
                bat 'dotnet test TestProject2/TestProject2.csproj --no-build --verbosity normal'
            }
        }
        stage('Dotnet test Project 3') {
            steps {
                bat 'dotnet test TestProject3/TestProject3.csproj --no-build --verbosity normal'
            }
        }
    }
}