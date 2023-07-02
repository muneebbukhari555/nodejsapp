pipeline {				
    agent any				
    triggers {				
        pollSCM('* * * * *')				
    }				
    stages {				
        stage('Build') {				
            steps {	
                checkout([$class: 'GitSCM', 				
				branches: [[name: "origin/master"]], 
				userRemoteConfigs: [[
                url: 'https://github.com/muneebbukhari555/nodejsapp.git']]])
            }				
        }				
    }				
}
