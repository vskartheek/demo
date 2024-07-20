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
                echo 'Install webserver'
            }
        }
	 stage('deploy app') {
            steps {
                echo 'deploy app'
            }
        }
    }
}
