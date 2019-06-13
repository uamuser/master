pipeline {
    agent any
	 environment {
                JIRA_HOME = 'C:/Atlassian/home'
                JAVA_HOME = 'C:\\Java\\jre1.8.0_211'
                JRE_HOME = 'C:\\Java\\jre1.8.0_211'
            }
    stages {
        stage('installation') {
            steps {
                sh '''
                mkdir C:/Atlassian
                mkdir C:/Atlassian/home
                cp -r C:/shared/jdk1.8 C:/java 
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
