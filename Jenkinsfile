Pipeline {
    agent any
    stages {
        stage ('checkout') {
            steps {
                echo 'checkout successfully'
            }
           

        }
        stage ('build') {
            steps {
                echo 'built successfully'
            }
        }
        stage ('test') {
            steps {
                echo 'tested successfully'
                
            }
        }
        stage ('deploy') {
            steps {
                echo 'deployed successfully'
            }
        }
    }
    post {
        always {
            echo 'this will always run'
        }
        success {
            echo 'this will only run if successful'
        }
        failure {
            echo 'this will only run if failed'
        }
        unstable {
            echo 'this will only run if the run is marked as unstable'

        }
        changed {
            echo 'this will only run if the state of the pipeline has changed'
            echo 'for example, if the pipeline was previously failed but now successful'
        }
    }
}
