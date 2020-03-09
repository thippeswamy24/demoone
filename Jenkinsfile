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
                sh 'sudo rm -rf /home/ec2-user/newdirectory'
                sh 'sudo rm -rf *;sudo git clone https://github.com/thippeswamy24/jenkins-terraform.git /home/ec2-user/newdirectory'
                //sh 'cd '
                //dir(' /one ') {
                   // checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [[$class: 'RelativeTargetDirectory', relativeTargetDir: '/root/demo']], submoduleCfg: [], userRemoteConfigs: [[]]])
                   // sh 'rm -rf *;git clone https://github.com/thippeswamy24/jenkins-terraform.git'
                  //  sh 'chmod 777 jenkins-terraform'
                 // sh 'mv -vf /var/lib/jenkins/workspace/swamy/jenkins-terraform /home/ec2-user/one'
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
