pipeline {
    agent any

    environment {
		JIRA_HOME= 'C:/Atlassian/home'
        JAVA_HOME = 'C:\\Program Files (x86)\\Java\jre1.8.0_211'
        JRE_HOME  = 'C:\\Program Files (x86)\\Java\\jre1.8.0_211'
    }

    stages {
        stage('Build') {
            steps {
                bat 'set'
				echo "PATH=${JAVA_HOME}"
            }
        }
    }
}
