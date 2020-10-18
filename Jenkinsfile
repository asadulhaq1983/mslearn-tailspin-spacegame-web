node(){
  stage("Checking Out Repo") {
   checkout scm
  }
  echo "${WORKSPACE}"
  echo "${BRANCH_NAME}"
  stage("Zipping"){
    //def b="${BRANCH_NAME}"
    //if(b=='master')
      // {
    zip zipFile:'a.zip', dir:'.'
  //}
  //else {
  //zip zipFile:"b.zip"
  //}
  
  }
}
