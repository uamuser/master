pipeline {
    agent any

    environment {
		JIRA_HOME= 'C:/Atlassian/home'
        JRE_HOME  = 'C:\\Program Files (x86)\\Java\\jre1.8.0_211'
    }

    stages {
        stage('Build') {
            steps {
                bat 'set'
		    if (env.JAVA_HOME=''){
			    JAVA_HOME = 'C:\\Program Files (x86)\\Java\\jdk1.8.0_211'
        	    }
		    if (env.JRE_HOME=''){
			    JRE_HOME = 'C:\\Program Files (x86)\\Java\\jre1.8.0_211'
        	    }

            }
        }
    }
}
