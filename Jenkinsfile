
pipeline {
    agent any
    stages {
        stage ('Example') {
            steps {
                echo "cloning git repo"
                git credentialsId: 'shakeersreboot', url: 'https://github.com/gitjenkins-cicd/Testgitpush.git'
                }
            }
        }
    }
