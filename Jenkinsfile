pipeline{
	agent any
	stages{
	
		stage('building'){
			steps{
				echo 'compilando proyecto'
				sh 'npm install'
				sh 'npm run build'
			}
		}
		
		stage('copy files'){
			steps{
				echo 'copiando ficheros'
				sh 'cp -r dist/* /var/www/html/ProyectoReact/'
			}
		}
		
	}

}
