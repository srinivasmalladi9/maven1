node('master')
{
    stage('continuousDownload')
    {
        git 'https://github.com/intelliqittrainings/maven.git'
    }
    stage('continuousBuild')
    {
        sh label: '', script: 'mvn package'
    }
}
