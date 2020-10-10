node('master')
{
    stage('continuousDownload')
    {
        git 'https://github.com/intelliqittrainings/maven.git'
    }
    stage('ContinuousBuild') 
    {
        sh label: '', script: 'mvn package'
    }
    stage('continuousdeployment')
    {
        stage('continuousdeployment')
    {
        scp /home/ubuntu/.jenkins/workspace/scripted/webapp/target/webapp.war ubuntu@172.31.2.79:/var/lib/tomcat8/webapps/test.war
    }
        stage('continuousTesting') 
    {
      git 'https://github.com/intelliqittrainings/FunctionalTesting.git'
      sh 'cd /home/ubuntu/.jenkins/workspace/b/testing.jar'
    }
}
