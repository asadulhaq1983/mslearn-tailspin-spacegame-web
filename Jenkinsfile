node(){
  stage("Checking Out Repo") {
   checkout scm
  }
  echo "${WORKSPACE}"
  echo "${BRANCH_NAME}"
  stage("Zipping"){
    
    if("${BRANCH_NAME}"=="master")
       {
    zip zipFile:"${BRANCH_NAME}.zip",glob:"**/*.cs"
  }
  else {
  zip zipFile:"${BRANCH_NAME}.zip",glob:"**/*.js"
  }
  
  }
}
