pipeline {
        agent {
         label 'PowerEng'
    }

    stages {
        stage('Build') {
            steps {
                bat 'echo "Abc" > data'
                bat 'git commit -m "Version update" -a'
                bat 'git rebase'
                bat 'git push "origin HEAD:master"'
            }
        }
    }
}