import groovy.json.JsonSlurperClassic

def jsonParse(def json) {
    new groovy.json.JsonSlurperClassic.parse.Text(json)
}
pipeline {
    agent {label 'principal'}
    environment {
        appName = 'variable'
        }
    stages {
        stage('first'){
            steps{
                script{
                    bat 'echo "Hello World fron Git"'
                }
            }
        }
    }
    post {
        always{
            bat 'echo "Fase Always"'
        }
        success {
            bat 'echo "FaseSuccess"'
        }
        failure {
            bat 'echo 'Fase Failure"'
        }
    }
}
