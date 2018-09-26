pipeline {
        agent {
         label 'PowerEng'
    }

    stages {
        stage('Build') {
            steps {
                bat 'echo "Abc" > data'
                bat 'git commit'
                bat 'git push'
            }
        }
    }
}