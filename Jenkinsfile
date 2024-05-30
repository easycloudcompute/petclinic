pipeline {
	agent any
    stages {
        stage('Build on eks') {
            steps {           
                        sh 'pwd'
                        sh 'cp -R helm/* .'
		        sh 'ls -ltr'
                        sh 'pwd'
                        sh '/usr/local/bin/helm upgrade --install petclinic-app petclinic  --set image.repository=cloudfreak.azurecr.io/cloudfreak/petclinic --set image.tag=1'
              			
            }           
        }
    }
}
