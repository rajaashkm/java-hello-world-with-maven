pipeline{
    agent any
    stages{
        stage("clone code"){
            steps{
                git 'https://github.com/rajaashkm/java-hello-world-with-maven.git'
            }
        }
        stage("Build"){
            steps{
                sh "mvn clean package"
            }
        }
    }
}
