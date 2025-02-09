pipeline {
    agent any
    tools {
       go 'go-1.23.6' // Comes from the jenkins global config
    
    }

    stages {
        stage('Build') {
            steps {
                sh 'bash scripts/build.sh' // Run the build
            }
        }
        stage('Test') {
            steps {
                sh 'bash scripts/test.sh' // Run the test
            }
        }
    }
}
