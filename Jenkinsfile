pipeline {
    agent any

    stages {
        stage('Compile') {
            steps {
                echo 'Hello World'
				atlas-compile
            }
        }
		 stage('Package') {
            steps {
                echo 'Hello World'
				atlas-package

            }
        }
		 stage('Deploy') {
            steps {
                echo 'Hello World'
				atlas-install-plugin --username babumungar --password Babu@99908 --server localhost --http-port 8080 --plugin
				-key com.atlassian.jira.jira-api --context-path ""
            }
        }
    }
}
