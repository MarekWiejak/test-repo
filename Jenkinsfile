pipeline {
    agent any
    
    environment {
        DISASBLE_AUTH = 'true'
        DB_ENGINE
    }
    
    stages {
        stage('build') {
            steps {
                sh 'python --version'
                sh 'echo "Hello World"'
                sh '''
                    echo "Multiline shell steps"
                    ls -lah
                '''
                echo "Database engine is ${DB_ENGINE}"
                echo "DISABLE_AUTH IS ${DISABEL_AUTH}"
                sh 'printenv'
            }
        }
    }
}
