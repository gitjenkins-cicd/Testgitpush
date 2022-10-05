
pipeline {
    agent any
    stages {
        stage ('Example') {
            steps {
                echo "cloning git repo"
                git branch: 'main', credentialsId: 'shakeersreboot', url: 'https://github.com/gitjenkins-cicd/Testgitpush.git'
                //sh "wget http://archive.apache.org/dist/tomcat/tomcat-8/v8.0.23/bin/apache-tomcat-8.0.23.tar.gz"
                //sh "git push branch: 'main', credentialsId: 'shakeersreboot', url: 'https://github.com/gitjenkins-cicd/Testgitpush.git'"
                sh "git tag -a 20 -m 'merging downloads'"
                //sh 'git merge main'
                sh "git add -A"
                //sh "git commit -am 'Merged develop branch to main'"
                sh "git remote add origin https://github.com/gitjenkins-cicd/Testgitpush.git"
                sh "git push --set-upstream origin main"
                sh "ls -a"
                }
            }
        }
    }
