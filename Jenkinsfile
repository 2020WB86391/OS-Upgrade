pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/2020WB86391/Ubuntu_Upgrade.git'
            }
        }
        stage('Run Ansible Playbook') {
            steps {
                ansiblePlaybook installation: 'Your-Ansible-Installation-Name', playbook: 'upgrade2.yml'
            }
        }
    }
}pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/2020WB86391/Ubuntu_Upgrade.git'
            }
        }
        stage('Run Ansible Playbook') {
            steps {
                ansiblePlaybook installation: 'Your-Ansible-Installation-Name', playbook: 'upgrade2.yml'
            }
        }
    }
}
