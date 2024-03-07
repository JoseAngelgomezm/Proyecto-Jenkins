pipeline{
	agent any
	
	stages{
	
		stage("building"){
			steps{
				echo "compilando proyecto"
				npm install
				npm run build
			}
		}
		
		stage("copy files"){
			steps{
				echo "copiando ficheros"
				sudo cp -r /dist/* /var/www/html/ProyectoReact/
			}
		}
		
	}

}
