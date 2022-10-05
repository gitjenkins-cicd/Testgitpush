
pipeline {
    agent any
    stages {
        stage ('Example') {
            steps {
                echo "cloning git repo"
                git branch: 'main', credentialsId: 'shakeersreboot', url: 'https://github.com/gitjenkins-cicd/Testgitpush.git'
                //sh "wget http://archive.apache.org/dist/tomcat/tomcat-8/v8.0.23/bin/apache-tomcat-8.0.23.tar.gz"
                git push https://github.com/gitjenkins-cicd/Testgitpush.git
                sh "ls -a"
                }
            }
        }
    }
