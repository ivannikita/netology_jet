 pipeline {
        agent { label 'molecule' }
        stages {
            stage('clone repo') {
                steps {
                    // sh '''
                    git branch: 'main', url: 'https://github.com/ivannikita/vector-role.git'
                    // '''
                    }}
            stage('install role by  galaxy') {
                steps {
                    sh '''
                    ansible-galaxy role install git+https://github.com/ivannikita/vector-role.git
                    '''
                    }}
            stage('run molecule test') {
                steps {
                    sh '''
                    molecule test
                    '''
                    }}
                }
    post {
        always {
        cleanWs()
        }
    }
    }