pipeline {
    agent any

    stages {
        stage('Check Git Rep') {
            steps {
                checkout scmGit(branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/raajaws/hello-world.git']])
            }
        stage('Build Project') {
            steps {
                sh "mvn clean install"
            }            
        }
    }
}
