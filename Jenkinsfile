pipeline {

	agent slave
		
		stages {
		
			stage("build") {
			
				steps {
					mkdir spring-petclinic
					git branch: 'main', url: 'https://github.com/spring-projects/spring-petclinic.git'
					cd spring-petclinic
					./mvnw package
				}
			}
		}				
}
