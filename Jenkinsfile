pipeline{
    agent none
    stages{
        stage('Maven Install'){
            agent { docker {'maven:3.5.0'} }
        }
        steps{
            sh 'mvn clean install'
        }
    }
}