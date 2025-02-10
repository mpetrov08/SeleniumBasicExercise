pipeline {
    agent any
    environment {
        CHROMEWEBDRIVER = '/usr/bin/google-chrome'
    }
    stages {
        stage('Build Project') {
            steps {
                bat 'dotnet build'
            }
        }
        stage('Run TestProject1 Tests') {
            steps {
                echo 'Running TestProject1 tests'
                bat 'dotnet test TestProject1/TestProject1.csproj --verbosity normal'
            }
        }
        stage('Run TestProject2 Tests') {
            steps {
                echo 'Running TestProject2 tests'
                bat 'dotnet test TestProject2/TestProject2.csproj --verbosity normal'
            }
        }
        stage('Run TestProject3 Tests') {
            steps {
                echo 'Running TestProject3 tests'
                bat 'dotnet test TestProject3/TestProject3.csproj --verbosity normal'
            }
        }
    }
}
