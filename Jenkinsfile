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
				sh 'mvn exec:java -Dexec.mainClass="com.maven.proyecto.App"'
			}
		}
		stage('end') {
			steps {
				echo 'Tarea2: finalizada con exito!!!'
			}
		}
	}
}
