node {
	stage ('SCM checkout'){
		git "https://github.com/Jeevan-Palo/BDD_Framework_Selenium_Java"
		}
	stage ('Build'){
    	dir("comtest") {
	   sh "mvn clean install"
       }
       	dir("comtest/target") {
	   sh "java -jar com.test-1.0-SNAPSHOT.jar"
       }
		}
}
