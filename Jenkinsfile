pipeline {
    agent {
        label ('NODE')
    }

    stages {
        stage ('Clone') {
            steps {
                git branch: 'main', url: "https://github.com/GUDAPATIVENKATESH/js-e2e-express-server.git"
            }
        }
        stage ('Install') {
            steps {
                sh 'export "PATH=/home/ubuntu/.nvm/versions/node/v16.14.0/bin:$PATH" '
                sh 'npm install'
            }
        } 
    }
}