pipeline {
    agent any

    parameters {
        choice(
                name: 'branch',
                choices: env.BRANCH_NAME,
                description: 'Branch to build'
        )
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
