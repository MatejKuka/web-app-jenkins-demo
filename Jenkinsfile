pipeline {
    agent any
    triggers {
        pollSCM("* * * * *")
    }
    stages {
        stage('Build') {
            steps {
                sh 'dotnet build'
                echo "Building..."
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
}