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
					accessToken: 'eyJ2ZXIiOiIyIiwidHlwIjoiSldUIiwiYWxnIjoiUlMyNTYiLCJraWQiOiJfR1RFQktHUTdUNW1mMWpCRXNxd0dpeHRvOVFUT2pBNnoyMER2WEFVbU44In0.eyJzdWIiOiJhZG1pbiIsInNjcCI6ImFwcGxpZWQtcGVybWlzc2lvbnNcL2FkbWluIGFwaToqIiwiYXVkIjoiamZydEAqIiwiaXNzIjoiamZmZUAwMDAiLCJpYXQiOjE1OTgxMTAyMzMsImp0aSI6IjI3YzUzMmI3LTE1ZTctNDMwYi1iZTY1LTdjNzI0MzBlNmJmMCJ9.c01pIAyiVwdcI_ynSLCzJr6c2xYSLi3vAfv64B0u7bA3jbGeqRtJpl8I8izjGoK0wPP4sVbrPXYj7C8S-m7w82fLkY6m_jZcbmqNVq0HzrBf2hdp_QU3bBnaLpGFHnwFvS8ICrfM8IFUFFFdfLpqBIhGAVLdiLHqiKbvbB__75hfI48gScA8ErRnZSSH9rHOlrWaPnVgKjvJSCgZXJ0PEyq3q8zr_lqyLyRn_-W9MWT_fIh032XNHhlGVcF165RK-pytfqgrzcpCXdNrb7dt02HwSWQtfu6L4SXpt0kdbARB0ErJEQaDFbDItmF00LOcSKWO2Oiu25SL5b90Yz57Aw'
				)
			}
		}
	}
}