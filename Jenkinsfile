node('master')
{
    stage('continuousdownload')
    {
            git 'https://github.com/intelliqittrainings/maven.git'
    }
    stage('continuousbuild')
    {
        sh label: '', script: 'mvn package'
    }
    stage('continuousdeployment')
    {
        scp /home/ubuntu/.jenkins/workspace/scripted/webapp/target/webapp.war ubuntu@172.31.39.87:/var/lib/tomcat8/webapps/test.war
    }
}
