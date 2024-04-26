pipeline {
agent any
 stages{
 stage('Git Checkout') {
    steps {
 checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/Mattaparthi321/java-web-project/edit/Release1']])
 echo 'Git Checkout Completed'
            }
        }


	 
 stage ('Build') {
            steps {
                sh "mvn clean package -Dmaven.test.failure.ignore=true"
	    }
 }
}
}
