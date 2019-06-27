pipeline {
    agent any
	 environment {
                JIRA_HOME = 'C:/Atlassian/home'
                JAVA_HOME = 'C:/java/jdk1.8'
                JRE_HOME = 'C:/java/jdk1.8/jre'
            }
    stages {
	    
       	stage('Apache-installation') {
		steps {
                sh '''
                mkdir C:/Software
				cp -r C:/shared/Apache C:/Software
				cd C:\Software\Apache24\bin
				httpd -k install
                '''
            }
        
		}
	    
	    
	}
}
