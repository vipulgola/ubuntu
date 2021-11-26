pipeline{
    agent any
    stages{
        stage('Clean stage'){
            steps{
                sh 'sudo docker pull dockerfile/ubuntu'
            }
        }
        stage('Build stage'){
            steps{
                sh 'docker build -t="vipulgola/ubuntu" github.com/dockerfile/ubuntu'
            }
        }
        stage('package'){
            steps{
                echo 'sudo docker push vipulgola/ubuntu'
            }
        }
        stage('package upload'){
            steps{
                echo 'Package upload'
            }
        }
    }
}
