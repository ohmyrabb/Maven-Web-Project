#!groovy

node {   
	stage('Checkout from GITHUB'){

          checkout scm
       }

       stage('BuildArtifact'){

         // sh 'mvn install'
	       
	       bar 'mvn clean package'
       }
	   
     /* stage('Sonar') {
                    //add stage sonar
                    sh 'mvn sonar:sonar'
                }*/
       
}
