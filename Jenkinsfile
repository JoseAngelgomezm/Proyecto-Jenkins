pipeline{
	agent any
	
	stages{
	
		stage("building"){
			steps{
				npm run build
			}
		}
		
		stage("copy files"){
			steps{
				sudo cp -r /dist/* /var/www/html/ProyectoReact/
			}
		}
		
	}

}
