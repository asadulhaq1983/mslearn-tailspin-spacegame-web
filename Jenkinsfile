node(){
  stage("Checking Out Repo") {
   checkout scm
  }
  echo "${WORKSPACE}"
  echo "${BRANCH_NAME}"
  stage("Zipping"){
    
    if("${BRANCH_NAME}"=="master")
       {
    zip zipFile:"a.zip"
  }
  else {
  zip zipFile:"b.zip"
  }
  
  }
}
