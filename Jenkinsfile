pipeline {
    agent {
        node {
            label 'master'
        }
    }

    stages {

        stage('terraform started') {
            steps {
                sh 'echo "Started...!" '
            }
        }
        stage('dire') {
            steps {
                //sh 'cd '
                //dir(' /one ') {
                    sh label: '', script: '''cd /home/ec2-user/newfolder
                    git clone https://github.com/thippeswamy24/jenkins-terraform.git'''
                   // sh 'rm -rf *;git clone https://github.com/thippeswamy24/jenkins-terraform.git /home/ec2-user/newfolder'
                    
                  //  sh 'mv -v /var/lib/jenkins/workspace/swamy/jenkins-terraform /home/ec2-user/one'
               // }
            }
        }
        
   /*     stage('git clone') {
            steps {
                sh 'rm -r *;git clone https://github.com/thippeswamy24/jenkins-terraform.git'
            }
        }
        stage('tfsvars create') {
            steps {
                sh 'cp /home/ec2-user/vars.tf ./jenkins/'
            }
        }
        stage('terraform init') {
            steps {
                sh 'sudo /home/ec2-user/terraform init ./jenkins'
            }
        }
        stage('terraform plan') {
            steps {
                sh 'ls ./jenkins; sudo /home/ec2-user/terraform plan ./jenkins'
            }
        }
        stage('terraform ended') {
            steps {
                sh 'echo "Ended....!!"'
            }
        }
*/
        
    }
}
