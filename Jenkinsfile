pipeline {
	agent any
    stages {
        stage('Build on k8 ') {
            steps {           
                        sh 'pwd'
                        sh 'cp -R helm/* .'
		        sh 'ls -ltr'
                        sh 'pwd'
                        sh '/usr/local/bin/helm upgrade --install petclinic-app petclinic1  --set image.repository=registry.hub.docker.com/akhil1113/image1 --set image.tag=1'
              			
            }           
        }
    }
}
