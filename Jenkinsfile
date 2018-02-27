// Powered by Infostretch 

timestamps {

node () {

	stage ('Dhanush_Scal_Test_job1 - Checkout') {
 	 checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'Elazouzi', url: 'https://github.com/Elazouzi/Cloudera_Jenkins_test.git']]]) 
	}
	stage ('Dhanush_Scal_Test_job1 - Build') {
 	
// Unable to convert a build step referring to "jenkins.plugins.publish__over__ssh.BapSshPostBuildWrapper". Please verify and convert manually if required.
// Unable to convert a build step referring to "org.jvnet.hudson.plugins.SSHBuildWrapper". Please verify and convert manually if required.		// Shell build step
sh """ 
sbt package

sbt run 
 """ 
	}
}
}