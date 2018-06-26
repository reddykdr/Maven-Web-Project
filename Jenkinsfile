#!groovy

node {
	   
	stage('Checkout'){

          checkout scm
       }

       stage('BuildArtifact'){

          bat 'install'
       }
	   
      stage('Sonar') {
                    //add stage sonar
                    bat 'sonar:sonar'
                }
       
}
