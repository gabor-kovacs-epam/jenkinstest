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
                echo 'Building...'
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
