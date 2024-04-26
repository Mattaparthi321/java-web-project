pipeline {
agent any
 stages{
  stage ('clone') {
    		  steps {
                // clone the repo, go to snippet generator
                sh git clone https://github.com/Mattaparthi321/java-web-project.git
								}
               
            }
  
 stage ('Build') {
            steps {
                sh "mvn clean package -Dmaven.test.failure.ignore=true"
               
            }
  
 }

}
}




