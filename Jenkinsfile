stage "Docker Build"

node {
   git "https://github.com/ananthfrancis/test-pipeline.git"
   sh "docker build ."
}

stage "test on supported OSes"

parallel (
  windows: { node {
    sh "echo building on windows now"

 }},
  mac: { node {
    sh "echo building on mac now"
 }} )
