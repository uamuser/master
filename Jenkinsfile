pipeline {
    agent any

    environment {
		JIRA_HOME= 'C:/Atlassian/home'
JRE_HOME = 'C:\\Program Files (x86)\\Java\\jre1.8.0_211'        
    }

    stages {
        stage('Build') {
            steps {
		    script{
                bat 'set'
		    if (env.JAVA_HOME==''){
			    echo 'java home found'
			    JAVA_HOME = 'C:\\Program Files (x86)\\Java\\jdk1.8.0_211'
        	    }
		    if (env.JRE_HOME==''){
			    echo 'jre home not found'
			    JRE_HOME = 'C:\\Program Files (x86)\\Java\\jre1.8.0_211'
        	    }
		    }
            }
        }
    }
}
