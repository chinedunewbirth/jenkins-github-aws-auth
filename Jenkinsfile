pipeline {
    agent any
    stages {
        stage('Clone Repo') {
            steps {
                sshagent(['github-ssh-key']) {
                    git branch: 'main', credentialsId: 'github-ssh-key', url: 'git@github.com:chinedunewbirth/jenkins-github-aws-auth.git'
                }
            }
        }

        stage('Build') {
            steps {
                echo 'Cloned using SSH!'
            }
        }
    }
}
