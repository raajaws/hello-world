pipeline {
    agent any

    stages {
        stage('Check Git Rep') {
            steps {
                checkout scmGit(branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/raajaws/hello-world.git']])
            }
        }
<<<<<<< HEAD
        stage('Build Project') {
            steps {
                //sh "mvn clean install"
                echo "Build Project"
            }            
        }
    }
=======
     }
>>>>>>> bf71f826efa5fb563ab3528160ebd61925ef65ba
}
