#!groovy

node {   
	stage('Checkout from GITHUB'){

          checkout scm
       }

       stage('BuildArtifact'){

         // sh 'mvn install'
	       
	       bat 'mvn clean package'
       }
	   
     /* stage('Sonar') {
                    //add stage sonar
                    sh 'mvn sonar:sonar'
                }
       
       stage('deploying artifacts into nexus'){

         // sh 'mvn install'
	       
	       bat 'mvn clean deploy'
       }*/
	
	
       stage('Deploying to tomcat'){
        bat copy C:\Users\Rabbani\.jenkins\workspace\MavenPipelineProject\target\maven-web-project-1.1.war C:\Devops-Softwares\tomcat\apache-tomcat-9.0.10\webapps\
       }
}
