node {
       stage('git clone') {
        git credentialsId: 'dceb522d-8fe4-4b78-878e-b6bbd66c3f53', url: 'https://github.com/mbhavs/capgemini.git'    
    }            
    stage('mvn clean') {
        sh'mvn clean'
	}
	stage('mvn validate') {
	    sh 'mvn validate'
	}
	stage('mvn compile') {
	    sh 'mvn compile'
	}
	stage('mvn test') {
	    sh 'mvn test'
	}
	stage('mvn package') {
	    sh 'mvn package'
	}
}