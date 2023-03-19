pipeline {
    agent any
    stages {
        stage('Other_Hello'){
            steps{
                script{
                    echo "Hello World from Git"
                }
            }
        }
    }
    post {
        always{
            echo "Fase Always"
        }
        success {
            echo "FaseSuccess"
        }
        failure {
            echo "Fase Failure"
        }
    }
}
