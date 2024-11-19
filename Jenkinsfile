pipeline {
    agent any

    stages {
        stage('Hello') {
            agent {
                docker {
                    image 'alpine'
                }
            }
            steps {
                sh 'printenv'
                sh 'env'
            }
        }
    }
}
