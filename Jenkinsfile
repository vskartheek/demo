pipeline {
    agent any

    stages {
        stage('Fetch code') {
            steps {
               git branch: 'main', url: 'https://github.com/vskartheek/demo.git'
            }
        }
    }
}
