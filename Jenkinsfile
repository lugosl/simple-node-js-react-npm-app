pipeline {
    agent {
        docker {
            image 'node:6-alpine'
            args '-p 3000:3000'
            args '-v $HOME/.m2:/root/.m2'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
    }
}
