pipeline {
	agent any
    stages {
        stage('Build on k8 ') {
            steps {           
                        sh 'pwd'
                        sh 'cp -R helm/* .'
		        sh 'ls -ltr'
                        sh 'pwd'
		        sh 'helm repo update'
                        sh '/usr/local/bin/helm upgrade --install ishaan-app ishaan18  --set image.repository=registry.hub.docker.com/akhil1113/ishaan18 --set image.tag=1'
              			
            }           
        }
    }
}
