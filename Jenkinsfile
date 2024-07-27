pipeline {
	agent any
	stages {
		stage('Hello'){
			steps{
				echo "Hello from MAIN branch"
			}
		}
	}
}

pipeline {
	agent any
	stages {
		stage('Hello'){
			steps{
				echo "Hello from DEMO branch"
			}
		}
		stage('print demo.txt'){
			when {
				branch "demo*"
			}
			steps{
				sh 'cat demo.txt'
			}
		}
	}
}
