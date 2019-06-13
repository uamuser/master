pipeline {
    agent any
    stages {
        stage('installation') {
            steps {
                sh '''
                mkdir C:/Atlassian
                mkdir C:/Atlassian/home
                cp -r C:/shared/jdk* C:/java 
                cp -r C:/shared/jira C:/Atlassian
                '''
            }
        }
    }
    stages('check and start') {

        stage(Environment variable '){
            environment {
                JIRA_HOME = 'C:/Atlassian/home'
                JAVA_HOME = 'C:\Java\jre1.8.0_211'
                JRE_HOME = 'C:\Java\jre1.8.0_211'
            }
        }

        stage('start jira') {
            steps {
                bat ' C:\Atlassian\jira\bin\start-jira.bat'

            }
        }



    }



}
