stage "Docker Build"

node {
   git "https://github.com/ananthfrancis/test-pipeline.git"
   sh "docker build ."
}

input message: 'Do you want to deploy in UAT', ok: 'Okay', submitter: 'test' 

stage "UAT Deployment"
node {
   git "https://github.com/ananthfrancis/test-pipeline.git"
   sh "docker build ."
}
