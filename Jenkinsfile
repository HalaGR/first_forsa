pipeline {

	agent any //run code with agent slave
		
		stages {
		
			stage("build") { // stage Build
			
				steps {
					git branch: 'main', url: 'https://github.com/spring-projects/spring-petclinic.git' //clone repo
					dir('spring-petclinic') { //do in directory spring-petclinic
						script{
							"./mvnw package"
						}
					}
				}
				
			}
			
		}
	
}
