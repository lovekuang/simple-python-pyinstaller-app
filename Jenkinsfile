pipeline {
    agent none 
    stages {
        stage('Build') { 
            agent { 
                node 
                { label 'master'} 
            }
            steps {
                bat 'python -m py_compile sources/add2vals.py sources/calc.py' 
            }
        }
    }
}
