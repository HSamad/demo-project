pipeline {
    agent {label "linux"} 
	options{
		buildDiscarder logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '5', daysToKeepStr: '', numToKeepStr: '5')
		disableConcurrentBuilds()
	}
    stages {
        stage('Hello') {
            steps {
                echo "Hello World"
                
            }
        }
        stage('cat README') {
			when {
				branch "feature-*"
			}
            steps {
				bat """
					cat README.md
				"""	
                
            }
        }
    }
}