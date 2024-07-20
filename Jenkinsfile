pipeline {
    agent any

    stages {
        stage('Fetch code') {
            steps {
               git branch: 'main', url: 'https://github.com/vskartheek/demo.git'
            }
        }
	 stage('Install webserver') {
            steps {
		ansiblePlaybook inventory: '/var/lib/jenkins/workspace/test/dev', playbook: '/var/lib/jenkins/workspace/test/playbook1.yml', vaultTmpPath: ''            }
        }
	 stage('deploy app') {
            steps {
                echo 'deploy app'
            }
        }
    }
}
