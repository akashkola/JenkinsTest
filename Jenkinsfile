pipeline {
    agent any

    parameters {
      text defaultValue: 'test', name: 'payload'
    }
    
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
                echo "$payload"
            }
        }
    }
}
