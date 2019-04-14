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
                        load(environment.groovy)
                echo "${MY_CREDS_USR}" 
                    }
                }
            }
        }
    }
}
