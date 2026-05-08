pipeline {
    agent any
parameters {
        choice(name: 'ENV', choices: ['dev', 'qa', 'prod'], description: 'Select environment')
    }
    stages {

        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/tharunamazon06-lab/git-practice.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building project...'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }
    }
}
