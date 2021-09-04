node ('Windows') {
	stage ('SCM checkout'){
		git "https://github.com/devshree5/selenium-Jenkinspipeline.git"
		}
	stage ('Build'){
    	dir("comtest") {
	   bat "mvn install"
       }
	}
    stage ('test') {
    	bat "java -jar comtest/target/com.test-1.0-SNAPSHOT.jar"
    }
}
