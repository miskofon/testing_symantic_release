pipeline {
    agent any
    git credentialsId: 'df9122db-c2cf-4b5e-9769-22db85bac5dc', url: 'ssh://tfs.eplan.lan:22/tfs/DefaultCollection/CUS%20GROM%20Team/_git/RSP.Tests'
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