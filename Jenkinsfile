pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'master', url: 'https://github.com/2020WB86391/OS-Upgrade.git'
            }
        }
        stage('Run Ansible Playbook') {
            steps {
                ansiblePlaybook installation: '/root/ansible-playbook', playbook: 'upgrade.yml'
            }
        }
    }
}

