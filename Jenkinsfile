node(){
  stage("Checking Out Repo") {
   checkout scm
  }
  echo "${WORKSPACE}"
  stage("Zipping"){
    
    if("${BRANCH_NAME}".contentEquals("master"))
       {
    zip zipFile:"${BRANCH_NAME}.zip",glob:"**/*.cs"
  }
  else {
  zip zipFile:"${BRANCH_NAME}.zip",glob:"**/*.js"
  }
  
  }
}
