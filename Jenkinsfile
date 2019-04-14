pipeline {
    agent any
    parameters {
  choice choices: ['one', 'two ', 'three'], description: '', name: 'CHOICES'
}
    stages {
        stage('Example stage 1') {
            steps {
                script {
                    if (CHOICES == 'one') {
                    creds = load(environment.groovy)
                    cred.MY_CREDS()
                echo "${MY_CREDS_USR}" 
                    }
                }
            }
        }
    }
}
