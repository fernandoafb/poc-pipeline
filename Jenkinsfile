pipeline {
    agent { docker { image 'node:6.3' } }
    stages { 
        stage('build') {
            steps {
                def dockerHome = tool 'docker-jenkins'
                env.PATH = "${dockerHome}/bin:${env.PATH}"
                sh 'npm --version'
            }
        }
    }
}