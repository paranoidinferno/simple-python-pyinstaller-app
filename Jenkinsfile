pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                sh 'python -m py_compile sourcesadd2vals.py sourcescalc.py' 
                stash(name 'compiled-results', includes 'sources.py') 
            }
        }
    }
}