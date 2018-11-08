pipeline {
	agent none
	stages {
		stage('Build') {
			agent {
				docker {
					image 'python:2-alpine'
				}
			}
			steps {
				sh 'python -m py_compile sources/add2bals.py sources/calc.py'
			}
		}
	}
}
