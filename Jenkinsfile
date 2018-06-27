#!groovy

node {
	   
	stage('Checkout'){

          checkout scm
       }

       stage('BuildArtifact'){
          // build step
	  echo "PATH = ${PATH}"
          echo "M2_HOME = ${M2_HOME}"     
          bat 'mvn install'
       }
	   
      stage('Sonar') {
                    //add stage sonar
                    bat 'mvn sonar:sonar'
                }
       
}
