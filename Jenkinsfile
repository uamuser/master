pipeline {
    agent any
    stages {
        stage('installation') {
            steps {
                sh '''
                mkdir C:/Atlassian
                mkdir C:/Atlassian/home
                cp -r C:/shared C:/java 
                '''
            }
        }
    }

}
