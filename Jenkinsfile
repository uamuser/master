pipeline {
    agent any
	 environment {
                JIRA_HOME = 'C:/Atlassian/home'
                JAVA_HOME = 'C:/java/jdk1.8'
                JRE_HOME = 'C:/java/jdk1.8/jre'
            }
    stages {
       	stage('installation') {
		steps {
                sh '''
                cp -r C:/shared/java C:/java
		'''
            }
        }
        
}
}
