pipeline {
	agent any
    stages {
        stage('Build on k8 ') {
            steps {           
                        sh 'pwd'
                        sh 'cp -R helm/* .'
		        sh 'ls -ltr'
                        sh 'pwd'
                        sh '/usr/bin/helm upgrade --install auth-services petclinic  --set image.repository=cloudfreak.azurecr.io/cloudfreak/petclinic --set image.tag=1'
              			
            }           
        }
    }
}
