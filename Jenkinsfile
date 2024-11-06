pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'master', url: 'https://github.com/2020WB86391/OS-Upgrade.git', credentialsId: 'git-credentials'
            }
        }
        stage('Run Ansible Playbook') {
            steps {
                ansiblePlaybook installation: '/root/ansible-playbook', playbook: 'upgrade.yml', extraVars: '@group_vars/all/vault.yml', vaultCredentialsId: 'vault-credentials-id'
            }
        }
    }
}

