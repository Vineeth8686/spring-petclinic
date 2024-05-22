pipeline{
    agent none
        stages{
        stage('Maven Build'){
        agent{
            docker{ image 'maven:3.5.0'}
        }
        steps{
            sh 'mvn clean install'
        }

        }

        stage("Docker Build"){
        agent any
        steps{
            sh "docker build -t vineeth8686/spring-petclinic:latest ."
        }
        }

        }
    
}