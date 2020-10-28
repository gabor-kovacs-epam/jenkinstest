pipeline {
    agent any

    parameters {
        gitParameter name: 'BRANCH_TAG', 
                     type: 'PT_BRANCH_TAG',
                     defaultValue: 'master'
    }
    
    stages {
        stage('Build') {
            steps {
                checkout([$class: 'GitSCM', 
                          branches: [[name: "${params.BRANCH_TAG}"]], 
                          doGenerateSubmoduleConfigurations: false, 
                          extensions: [], 
                          gitTool: 'Default', 
                          submoduleCfg: [], 
                          userRemoteConfigs: [[url: 'https://github.com/jenkinsci/git-parameter-plugin.git']]
                        ])
                echo 'Building...'
                echo '---------------------------------------'
                sh 'git status'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
            }
        }
    }
}
