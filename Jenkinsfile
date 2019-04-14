pipeline {
    agent any
  environment {
    load 'environment.groovy'
  }
    stages {
        stage('Example stage 1') {
            environment {
                MY_CREDS = credentials('MY_CREDS')
            }
            steps {
                echo "${MY_CREDS_USR}" 
            }
        }
    }
}
