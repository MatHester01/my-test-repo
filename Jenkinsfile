pipeline {
    agent any
  environment {
      parameters { choice(name: 'CHOICES', choices: ['one', 'two', 'three'], description: '') }
      if (CHOICES == 'one') {
    load 'environment.groovy'
      }
  }
    stages {
        stage('Example stage 1') {
            steps {
                echo "${MY_CREDS_USR}" 
            }
        }
    }
}
