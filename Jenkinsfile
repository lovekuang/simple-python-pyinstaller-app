pipeline {
    agent any 
    stages {
        stage('build') { 
            agent any
            steps {
                bat 'python -m py_compile sources/add2vals.py sources/calc.py' 
            }
        }
    }
}
