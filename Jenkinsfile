node 
{
    stage('Checkout')
    {
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'a6b21194-d00a-4a5e-bfc1-871b24391a21', url: 'https://github.com/alekhyagudimetla/movies_project.git']]])
        workspace = pwd()
    }
    stage('static code analysis'){
        echo 'static code analysis'
    }
    stage('Build'){
        echo 'build'
    }
    stage('unit test'){
        echo 'unitest'
    }
    stage('delivery'){
        echo 'delivery'
    }
}
