pipeline {
    agent any
    stages {
        stage('installation') {
            steps {
                sh '''
                mkdir C:\\Atlassian
                mkdir C:\\Atlassian\\home
                curl -o. /jira.zip https://product-downloads.atlassian.com/software/jira/downloads/atlassian-jira-software-8.2.1.zip
                unzip jira.zip -d C:\\Atlassian
                cp -r C:\\shared C:\\java 
                '''
            }
        }
    }

}
