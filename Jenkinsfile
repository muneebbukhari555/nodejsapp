node{
	def name="jeff"
	def isGroovyCool = false
    withEnv(['DEPLOY_TO=production']) {
        stage('Build') {
		
			//when-environment condition
			if(env.DEPLOY_TO == 'production')
				println "Deploying"
				
			//when-equals condition
			if(	env.BRANCH_NAME == "main")
				println "name is ${name}"

			//when-expression condition				
			if(	env.BRANCH_NAME == "main")
				println "groovy is always cool"
				
			//when-not condition
			if(	env.BRANCH_NAME == "main")
				println "name is not john"			
			
			//when-allOf condition			
			if(	env.BRANCH_NAME == "main")
				println "name is ${name} and groovy is cool"
				
			//when-anyOf condition	
			if(	env.BRANCH_NAME == "main")
				println "name is ${name} or groovy is cool"	
        }
    }
}
