pipeline{
    agent any
    stages{
        stage('Git clone'){
            steps{
                git branch: 'main', url: 'https://github.com/yulakhraj/maven_jenkins.git'
            }
        }
        
        stage('Maven Test'){
            steps{
                sh 'mvn test'
            }
        }
        
        stage('Maven Build'){
            steps{
                sh 'mvn package'
            }
        }
        
        stage('Maven Deploy'){
            steps{
                echo "deployed war file to the server"
            }
        }
    }
}
