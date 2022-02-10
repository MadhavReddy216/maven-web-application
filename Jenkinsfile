pipeline{

agent any

tools
{
  maven 'maven3.6.3'

}
 stages{
   
   stage('CheckoutCode from master')
   {
     steps{
	 git branch: 'master', credentialsId: '8e348aa2-9531-4dbe-863d-1adb64897470', url: 'https://github.com/MadhavReddy216/maven-web-application.git'
	 }
   }
   
   stage('Build from master')
   {
    steps{
	  sh "mvn clean package"
	 }
   }
 }
}
