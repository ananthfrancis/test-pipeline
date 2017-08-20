stage "unit test"

node {
   git "https://github.com/ananthfrancis/test-pipeline.git"
   sh "echo unit test app"
}

stage "test on supported OSes"

parallel (
  windows: { node {
    sh "echo building on windows now"

 }},
  mac: { node {
    sh "echo building on mac now"
 }}
