pipeline {
    agent none 
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
        
    }
}