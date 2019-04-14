pipeline {
    agent any
  environment {
    load 'environment.groovy'
  }
    stages {
        stage('Example stage 1') {
            steps {
                echo "${MY_CREDS_USR}" 
            }
        }
    }
}
