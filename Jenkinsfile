pipeline {
    agent any

    stages {
        stage('Run Ansible Playbook') {
            steps {
                bat 'wsl ansible-playbook -i /home/Frank-cloud/ansible-webserver/inventory.ini /home/Frank-cloud/ansible-webserver/playbook.yml'
            }
        }

        stage('Verify Deployment') {
            steps {
                bat 'wsl curl -s http://localhost'
            }
        }
    }

    post {
        success {
            echo 'Deployment successful!'
        }
        failure {
            echo 'Deployment failed!'
        }
    }
}
