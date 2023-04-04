pipeline 
{
    agent any

    stages 
    {
        stage('Check Git Rep') 
        {
            steps {
                checkout scmGit(branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/raajaws/hello-world.git']])
            }
        }
        stage('Build Project') 
        {
            steps {
                sh "export MAVEN_HOME=/opt/maven"
                sh "export PATH=$PATH:$MAVEN_HOME/bin"
                sh "mvn --version"
                sh "mvn clean package"
                sh "mvn clean install"
                echo "Build Project"
            }            
        }
    } 

}
