pipeline {
    agent any
	 environment {
                JIRA_HOME = 'C:/Atlassian/home'
                JAVA_HOME = 'C:/Java/jdk1.8'
                JRE_HOME = 'C:/Java/jdk1.8/jre'
            }
    stages {
       	steps {
                sh '''
                mkdir C:/Atlassian
                mkdir C:/Atlassian/home
                cp -r C:/shared/java C:/java/jdk1.8 
		cp -r C:/shared/jira C:/Atlassian
                '''
            }
        }
        stage('start jira') {
            steps {
                bat 'C:\\Atlassian\\jira\\bin\\start-jira.bat'
            }
    }
}
}
