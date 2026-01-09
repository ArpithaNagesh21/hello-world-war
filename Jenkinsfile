pipeline {
//agent { label 'Java_Env' }
  agent any 

    stages {
    
       stage('Checkout') {
            //agent { label 'Java_Env' }
            steps {

             withCredentials([
                    usernamePassword(
                        credentialsId: 'Git',
                        usernameVariable: 'USERNAME',
                        passwordVariable: 'PASSWORD'
                    )
                ])
             {
              sh 'echo welcome'
             sh 'echo $USERNAME $PASSWORD'
                //sh 'rm -rf *'
                //sh 'git clone https://github.com/ArpithaNagesh21/hello-world-war.git'
            }
            }
        }
    }
}
