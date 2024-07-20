pipeline {
    agent any

    stages {
        stage('Fetch code') {
            steps {
               git branch: 'main', url: 'https://github.com/vskartheek/demo.git'
            }
        }
                stage('Install web server') {
            steps {
             ansiblePlaybook credentialsId: 'cd1b772a-320b-4d2c-be2e-e38f58fcf7c1', disableHostKeyChecking: true, installation: 'Ansible', inventory: '/var/lib/jenkins/workspace/test/dev', playbook: '/var/lib/jenkins/workspace/test/playbook1.yml', vaultTmpPath: ''
            }
        }
    }
}
