pipeline {
	agent any
	stages {
		stage('init') {
			steps {
				echo 'Tarea2: iniciando'
			}
		}
		stage('test') {
			steps {
				sh 'mvn test'
			}
		}
		stage('package') {
			steps {
				sh 'mvn package'
			}
		}
		stage('execute') {
			steps {
				sh 'java -jar miPrimerProyecto-1.0-SNAPSHOT.jar'
			}
		}
		stage('end') {
			steps {
				echo 'Tarea2: finalizada con exito!!!'
			}
		}
	}
}
