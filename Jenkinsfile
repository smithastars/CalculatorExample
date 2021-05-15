pipeline {
	agent any
	tools {
    	maven 'myLocalMaven'
	}
	stages {
    	stage("Checkout") {   
        	steps {               	 
            	git branch:'main', url: 'https://github.com/smithastars/CalculatorExample.git'          	 
           	 
        	}    
    	}
    	stage('Build') {
        	steps {
        	sh "mvn compile"  	 
        	}
    	}
   	 
    	stage("Unit test") {          	 
        	steps {  	 
            	sh "mvn test"          	 
       	}
}
}
}
