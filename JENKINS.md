CICD


```bash
pipeline {
    agent {
        label 'linux'
    }

    environment {
        BUILD_ENV = 'production'
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building the project...'
                sh './build.sh'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                sh './test.sh'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                sh './deploy.sh'
            }
        }
    }
}
```
