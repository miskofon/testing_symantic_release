pipeline {
        agent {
         label 'PowerEng'
    }

    stages {
        stage('Build') {
            steps {
                bat 'echo "Abc" > data'
                bat 'git commit --author="RSP publisher"'
                bat 'git push'
            }
        }
    }
}