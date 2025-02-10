pipeline {
    agent any
    stages {
        stage('Build Project') {
            steps {
                bat 'dotnet build'
            }
        }
        stage('Run Project 1 Tests') {
            steps {
                bat 'dotnet test TestProject1/TestProject1.csproj'
            }
        }
        stage('Run Project 2 Tests') {
            steps {
                bat 'dotnet test TestProject2/TestProject2.csproj'
            }
        }
        stage('Run Project 3 Tests') {
            steps {
                bat 'dotnet test TestProject3/TestProject3.csproj'
            }
        }
    }
}