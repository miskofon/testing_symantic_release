pipeline {
        agent {
         label 'PowerEng'
    }

    stages {
        stage('Build') {
            steps {
			checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [[$class: 'LocalBranch', localBranch: 'master']], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'df9122db-c2cf-4b5e-9769-22db85bac5dc', refspec: '+refs/heads/master:refs/remotes/origin/master', url: 'ssh://tfs.eplan.lan:22/tfs/DefaultCollection/CUS%20GROM%20Team/_git/RSP.Tests']]])
                bat 'echo "Abc" > data'
                bat 'git commit -m "Version update" -a'
                bat 'git rebase master'
                bat 'git push "origin HEAD:master"'
            }
        }
    }
}