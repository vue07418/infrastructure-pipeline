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
    
    sh "aws ec2 run-instances --image-id ami-467ca739 --count 1 --instance-type t2.micro --key-name webserver --security-group-ids sg-814d35c8 --subnet-id subnet-908462be --region us-east-1"

    }
}
