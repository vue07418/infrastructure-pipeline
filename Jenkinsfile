properties([pipelineTriggers([githubPush()])])
node('linux') {
    git url: 
'https://github.com/vue07418/infrastructure-pipeline.git', branch: 
'master'
    stage('Test') {
        sh "env"
    }
}
