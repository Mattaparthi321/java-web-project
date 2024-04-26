pipeline {
agent any
 stages{
 stage ('Build') {
            steps {
                sh "mvn clean package -Dmaven.test.failure.ignore=true"
	    }
 }
}
}
