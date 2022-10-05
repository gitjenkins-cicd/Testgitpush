
pipeline {
    agent any
    stages {
        stage ('Example') {
            steps {
                echo "cloning git repo"
                git branch: 'main', credentialsId: 'shakeersreboot', url: 'https://github.com/gitjenkins-cicd/Testgitpush.git'
                sh "wget https://apachemirror.wuchna.com/tomcat/tomcat-8/v8.5.65/bin/apache-tomcat-8.5.65.tar.gz"
                sh "ls -a"
                }
            }
        }
    }
