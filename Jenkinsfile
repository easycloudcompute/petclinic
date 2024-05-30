pipeline {
	agent any
    stages {
        stage('Build on eks') {
            steps {           
                        sh 'pwd'
                        sh 'cp -R helm/* .'
		        sh 'ls -ltr'
                        sh 'pwd'
                        sh '/usr/local/bin/helm upgrade --install springboot-app-1 petclinic --set image.repository=rahulunixsa87/springboot-app-1 --set image.tag=2'              			
            }           
        }
    }
}
