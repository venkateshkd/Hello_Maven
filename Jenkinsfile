pipeline {
	agent { lable 'Node_Machine_37' } 
	stages {
	   stage ('Compile Stage'){
		steps {
		   withMaven(maven: 'maven'){
			sh 'mvn clean compile'
			}
		}
	}
 	
	
	stage ('Testing Stage'){
		steps {
		   withMaven(maven: 'maven'){
			sh 'mvn test'
			}
		}
	}
	
		
	 stage ('Deploy Stage'){
		steps {
		   withMaven(maven: 'maven'){
			sh 'mvn  deploy'
			}
		}
	}
   }

}
