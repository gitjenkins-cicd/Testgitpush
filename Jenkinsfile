
pipeline {
    agent any
    stages {
        stage ('Example') {
            steps {
                echo "cloning git repo"
                git branch: 'main', credentialsId: 'shakeersreboot', url: 'https://github.com/gitjenkins-cicd/Testgitpush.git'
                sh "ls -lrth"
                }
            }
        }
    }
