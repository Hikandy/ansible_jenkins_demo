pipeline {
    agent any
    stages {
        stage('running playbook') {
            steps {
                ansiblePlaybook becomeUser: 'ansible', colorized: true, disableHostKeyChecking: true, installation: 'ansible', inventory: 'inventory', playbook: 'lab8.yaml'
            }
        }
    }
}
