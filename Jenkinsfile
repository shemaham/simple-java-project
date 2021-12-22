pipeline {
    agent any

    stages {
        stage('github') {
            steps {
                sh "git clone https://github.com/shemaham/simple-java-project.git"
            }
        }
        stage('build') {
            steps {
                sh "cd /var/lib/jenkins/workspace/pipe/simple-java-project && mvn install"
            
            }
        }
        stage('deploy') {
            steps {
                echo "deploy"
            }
        }
    }
}
