pipeline{
    agent any
    stages {
        stage ("Welcome to the build") {
            steps{
                echo "First stage of the build"
            }
        }
        
        stage ("Checking out from GITHUB") {
            steps{
                git credentialsId: 'Git', url: 'https://github.com/chaitanyasaig/leadapp-maven.git'
            }
        }
        
        stage ("Input") {
            steps{
                input 'Shall we proceed?'
            }
            
        }
        
        }
    }
