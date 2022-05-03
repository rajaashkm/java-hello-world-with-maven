pipeline{
    agent any
    PATH = "/usr/share/maven:$PATH"
    stages{
        stage("clone code"){
            steps{
                git 'https://github.com/rajaashkm/java-hello-world-with-maven.git'
            }
        }
        stage("Build"){
            steps{
                sh "mvn clean test"
            }
        }
        stage("Build"){
            steps{
                sh "mvn package"
            }
        }
    }
}
