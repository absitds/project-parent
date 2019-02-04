pipeline {
    agent {
        docker {
            image '3.6-jdk-7-alpine' 
            args '-v /root/jenkins_home/.m2:/root/.m2' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn clean deploy -s /var/jenkins_home/.m2/settings.xml' 
            }
        }
    }
}
