pipeline {
	agent any
    stages {
        stage('Build on k8 ') {
            steps {           
                        sh 'pwd'
                        sh 'cp -R helm/* .'
		        sh 'ls -ltr'
                        sh 'pwd'
                        sh '/usr/bin/helm upgrade --install auth-services petclinic  --set image.repository=sanjeet1992/auth --set image.tag=1'
              			
            }           
        }
    }
}
