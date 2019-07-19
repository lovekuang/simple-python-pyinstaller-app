node {
    stage('Build') {
        if (env.BRANCH_NAME == 'master') {
            bat 'python -m py_compile sources/add2vals.py sources/calc.py' 
        } else {
            bat 'python -m py_compile sources/add2vals.py sources/calc.py' 
        }
    }
}
