pipeline {
	agent {
		label 'host'
	}
	stages {
		stage('Get http request') {
			steps {
				echo 'This is show you how to GET http request'
				echo 'echo list images of docker-local repo on jfrog'
				httpRequest (
					url: "http://192.168.168.1:8082/artifactory/docker-local",
					acceptType: 'TEXT_HTML',
					httpMode: 'GET',
					authentication: 'jfrogdeploy',  //user in credencial jenkins
					//requestBody: 'requestbody'
					consoleLogResponseBody: true,          //show body 
					outputFile: 'output-jfrog-repo.txt'   //extra contain to outputfile
				)
				sh 'cat ./output-jfrog-repo.txt'

			}
		}
	}
}

// info feature of http request : https://www.jenkins.io/doc/pipeline/steps/http_request/#http-request-plugin