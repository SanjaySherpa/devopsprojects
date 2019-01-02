node{
	stage('SCM Checkout'){
		git branch: 'smtpjenkins', url: 'https://github.com/SanjaySherpa/devopsprojects.git'
	}
	stage('Compile-Package'){
		def mvnHome = tool name: 'maven-3', type: 'maven'
		sh "${mvnHome}/bin/mvn package"
	}
	stage('Email Notification'){
	mail bcc: '', body: 'This is body', cc: '', from: 'prabhatiitbhu@gmail.com', replyTo: 'prabhatiitbhu@gmail.com', subject: 'This is Subject', to: 'prabhat@aptence.com'
	mail bcc: '', body: 'hello', cc: '', from: 'sherpasanjay11@gmail.com', replyTo: 'sherpasanjay11@hotmail.com', subject: 'whatsup', to: 'sherpasanjay11@hotmail.com'
	}

}
