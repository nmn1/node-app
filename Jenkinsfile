pipeline{
    agent any
    tools {
        nodejs 'Node-14.13.1'
    }

    environment{
        CI = 'true'
    }
        stages{
            stage('Build'){
                steps{
                    sh 'npm install'
                }
            }
            stage('Test'){
                steps{
                    sh './jenkins/scripts/test.sh'
                }
            }
        }
    
}