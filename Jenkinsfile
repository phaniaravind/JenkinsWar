/*Jenkinsfile for the maven project*/
pipeline {
        agent any
    environment {
            PATH = "/opt/maven-3.6.3/bin:$PATH"
    }
   stages {
        stage('Cloning Git') {
            steps {
                git credentialsId: 'git_credentials', url:'https://github.com/phaniaravind/JenkinsWar.git/'
            }
        }
        stage('Building') {
            steps {
                sh 'mvn clean package'
            }
        }
   }
