pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'this is Build step'
            }
        }
        stage('Test') {
            steps {
                echo 'this is Test step'
            }
        }
        stage('Deploy') {
            when {
                branch 'master'
            }
            steps {
                echo 'this is production Deploy step'
            }
        }
    }
    post { 
        always { 
            echo 'I will always say Hello again!'
        }
    }
}
