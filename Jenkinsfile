pipeline {

	agent slave
		
		stages {
		
			stage("build") {
			
				steps {
					mkdir spring-petclinic
					git clone https://github.com/spring-projects/spring-petclinic.git
					cd spring-petclinic
					./mvnw package
				}
			}
		}				
}
