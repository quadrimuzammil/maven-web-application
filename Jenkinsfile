node
{
    def mavenHome = tool name: "maven 3.8.4"
    stage ('code_checking')
    {
        git branch: 'development', credentialsId: '1f8cffd3-f04f-4b79-b692-55e6da7b046f', url: 'https://github.com/quadrimuzammil/maven-web-application.git'
    }
    
    stage ('Build_code')
    
    {
        sh "${mavenHome}/bin/mvn clean package"
    }
    /*
    stage ('Execute Code Quality Report')
    {
        sh "${mavenHome}/bin/mvn clean sonar:sonar"
    }
    stage ('Stored Atrifacts')
    {
        sh "${mavenHome}/bin/mvn clean deploy"
    }
    stage ('Deploy Application in Tomcat Server')
    {
    sshagent(['b4588750-ef52-4d11-9ccc-58c259e1639e']) 
    {
   sh"scp -o StrictHostKeyChecking=no target/maven-web-application.war ec2-user@13.233.36.216:/opt/apache-tomcat-9.0.58/webapps/"
    }
}
stage ('Email Notifications')
{
    mail bcc: '', body: '''Please find in server about application
Thanks & Regard
Quadri Muzammil
9922179697''', cc: '', from: '', replyTo: '', subject: 'Build over!', to: 'quadri.muzammil999@gmail.com'
}
*/



}
