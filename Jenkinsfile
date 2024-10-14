pipeline{
    agent any

    tools {
         maven 'maven'
         jdk 'jdk17'
    }

    stages{
        stage('iniatilize'){
            steps{
                echo "PATH = ${M2_HOME}/bin:${PATH}"
                echo "M2_HOME = /var/lib/jenkins/apache-maven*"
        }
        stage('build'){
            steps{
               dir("/var/lib/jenkins/workspace/toysstar") {
                sh 'mvn clean package'
            }
        }
    }
}
