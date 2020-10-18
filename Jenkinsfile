node(){
  stage("Checking Out Repo") {
   checkout scm
  }
  echo "${Build_Number}"
  def buildNo="${Build_Number}"
  echo "${WORKSPACE}"
  echo "${BRANCH_NAME}"
  def branchName="${BRANCH_NAME}"
  
  stage("Zipping"){
    
    if(branchName=='master')
       {
         zip zipFile:'Master_'+buildNo+'.zip', dir:'.'
  }
  else {
    zip zipFile:branchName+'_'+buildNo+'.zip'
  }
  
  }
}
