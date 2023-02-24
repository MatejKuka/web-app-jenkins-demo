pipeline {
    agent any
    
    triggers { 
    pollSCM '* * * * *' 
    }
    stages {
        stage('Build') {
            steps {
                sh "dotnet build web-app-jenkins-demo/web-app-jenkins-demo.csproj"
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