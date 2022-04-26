pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                git branch: 'main', url: 'https://github.com/marapo/AnsibleLabs.git'
                sh 'ansible-playbook playbook.yaml --extra-vars "text=$text"'
            }
        }
    }
}
