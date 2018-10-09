#!groovy

node {   
	stage('Checkout from GITHUB'){

          checkout scm
       }

       stage('BuildArtifact'){

         // sh 'mvn install'
	       
	       sh 'mvn clean package'
       }
	   
     /* stage('Sonar') {
                    //add stage sonar
                    sh 'mvn sonar:sonar'
                }*/
       
}
