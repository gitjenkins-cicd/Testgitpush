
pipeline {
    agent any
    stages {
        stage ('Example') {
            steps {
                echo "cloning git repo"
                git branch: 'main', credentialsId: 'shakeersreboot', url: 'https://github.com/gitjenkins-cicd/Testgitpush.git'
                //sh "wget http://archive.apache.org/dist/tomcat/tomcat-8/v8.0.23/bin/apache-tomcat-8.0.23.tar.gz"
                //sh "git push branch: 'main', credentialsId: 'shakeersreboot', url: 'https://github.com/gitjenkins-cicd/Testgitpush.git'"
                sh "git tag -a tagName -m 'merging downloads'"
                //sh 'git merge main'
                sh "git commit -am 'Merged develop branch to main'"
                sh "git push origin main"
                sh "ls -a"
                }
            }
        }
    }
