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
}
