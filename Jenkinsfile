pipeline {
    agent any
    stages{
        stage('scm checkkout'){
            steps{
                git branch: 'main', url: 'https://github.com/Hikandy/ansible_jenkins_demo'
            }
        stage('running playbook'){
            steps{
                ansiblePlaybook becomeUser: 'ansible', colorized: true, disableHostKeyChecking: true, installation: 'ansible', inventory: 'inventory', playbook: 'lab8.yaml'
            }
        }
    }
}
