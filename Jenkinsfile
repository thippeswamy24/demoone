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
        stage('change dir'){
        steps {
          sh "$PWD"
          dir('cd /root/opt'){
            sh "$PWD"
          }
        } 
      }
        stage('git clone') {
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

        
    }
}
