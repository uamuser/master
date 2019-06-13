pipeline {
    agent any
	 environment {
                JIRA_HOME = 'C:/Atlassian/home'
                JAVA_HOME = 'C:/Java/jre1.8.0_211'
                JRE_HOME = 'C:/Java/jre1.8.0_211'
            }
    stages {
       	
        stage('start jira') {
            steps {
                bat 'C:\\Atlassian\\jira\\bin\\start-jira.bat'
            }
    }
}
}
