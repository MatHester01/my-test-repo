pipeline {
    agent any
    parameters {
  choice choices: ['one', 'two ', 'three'], description: '', name: 'CHOICES'
}
    environment {
    def MY_CREDS;
    }
    stages {
        stage('Example stage 1') {
            steps {
                script {
                    if (CHOICES == 'one') {
                    env.MY_CREDS = credentials('MY_CREDS')
                        echo "Password is ${env.MY_CREDS_PSW}"
                        echo "Username is ${env.MY_CREDS_USR}"  
                    }
                }
                bat 'echo "Hello World"'
            }
        }
    }
}
