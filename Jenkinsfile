pipeline {
    agent any 
    stages {
        stage('build1') { 
            agent { label 'master' }
            steps {
                bat 'python -m py_compile sources/add2vals.py sources/calc.py' 
            }
		}
        stage('build2') { 
            agent { label 'jenkins-slaves-1' }
            steps {
                bat 'python -m py_compile sources/add2vals.py sources/calc.py' 
			}
		}
	}
}
