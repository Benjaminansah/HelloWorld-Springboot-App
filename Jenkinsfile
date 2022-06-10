pipeline {
    agent any
    stages{
        stage('Git clone'){
            steps{
                git branch: 'master', url: 'https://github.com/shazforiot/HelloWorld-Springboot-App.git'
            }
        }
        stage('Maven Build'){
            steps{
                sh 'mvn test'
            }
        }
        stage('Maven Deploy'){
            steps{
                sh 'mvn package'
            }
        }
        stage('Maven Test'){
            steps{
                echo " Deploying the war file to the server"
            }
        }
    }
}
