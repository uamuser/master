pipeline {
         agent any
         stages {
                 stage('installation') {
                 steps {
					sh '''
					mkdir C:\\Atlassian
					mkdir C:\\Atlassian\\home
                   			 curl -o ./jira.zip  https://product-downloads.atlassian.com/software/jira/downloads/atlassian-jira-software-8.2.1.zip
					unzip jira.zip -d C:/Atlassian
					'''
                 }
                 }
}

		stages('check and start'){
			  
			  stage(Environment variable'){
				environment {
				JIRA_HOME='C:/Atlassian/home'
				JAVA_HOME= 'C:\Java\jre1.8.0_211'
				JRE_HOME= 'C:\Java\jre1.8.0_211'
        }
}


			stage('start jira'){
				 steps{
				 bat ' C:\Atlassian\jira\bin\start-jira.bat'
				 
				 }
				 }
				 
				 
            
}

stage('DB connect') {
   when {
       not {
           user 'JIRAadminlogin'
       }
   }
   steps {
     	bat ' "sqlcmd -e -S \"(localdb)\\MyServer01\" -d \"JIRA_DB"\" -i \"C:\\test.sql\" -U \"JIRAadminlogin\" -P Accenture#1" '
							OR
	bat' sqlcmd -S myserver\instanceName -i C:\myscript.sql\" -U \"JIRAadminlogin\" -P Accenture#1" '
   }
}
}

 post {
        failure {    
            mail(to: 'me@example.com', subject: "Failed Pipeline", body: "Something is wrong.")
        }
		}

}
