pipeline {
    agent any
	 environment {
                JIRA_HOME = 'C:/Atlassian/home'
                JAVA_HOME = 'C:/Java'
                JRE_HOME = 'C:/Java/jre'
            }
    stages {
       	
        stage('start jira') {
            steps {
                bat 'C:\\Atlassian\\jira\\bin\\start-jira.bat'
            }
    }
}
}
