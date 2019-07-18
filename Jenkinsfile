pipeline {
    agent none 
    stages {
        stage('Build') { 
            agent { 
                node {
                    label 'master'
                    label1 'jenkins-slaves-1'
                }
            }
            steps {
                bat 'python -m py_compile sources/add2vals.py sources/calc.py' 
            }
        }
    }
}
