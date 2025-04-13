pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                sshagent(['github-ssh-key']) {
                    git url: 'git@github.com:your-username/your-repo.git', branch: 'main'
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
