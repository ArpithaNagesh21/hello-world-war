//agent { label 'Java_Env' }
  //  agent none

    stages {
     parallel {
      stage('Checkout')
     }
        stage('Checkout') {
            //agent { label 'Java_Env' }
            steps {

             withCredentials([
                    usernamePassword(
                        credentialsId: '9c077ca7-41a4-4545-a2b8-f0187fd29c66',
                        usernameVariable: 'USERNAME',
                        passwordVariable: 'PASSWORD'
                    )
                ])
             {
              sh 'echo welcome'
             sh 'echo $CMD $RUN_TESTS $CMD1'
             sh 'echo $USERNAME $PASSWORD'
                //sh 'rm -rf *'
                //sh 'git clone https://github.com/ArpithaNagesh21/hello-world-war.git'
            }
            }
        }
    }

