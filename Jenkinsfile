properties([pipelineTriggers([githubPush()])])
node('linux') {
    git url: 
'https://github.com/vue07418/infrastructure-pipeline.git', branch: 
'master'
    stage('Test') {
        sh "env"
    }
    
    stage ("GetInstances") {

    sh "aws ec2 describe-instances --region us-east-1"
    }

    stage ("CreateInstance") {
        // TODO

    }
}
