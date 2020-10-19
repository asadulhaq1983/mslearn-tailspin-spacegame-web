node(){
  stage("Checking Out Repo") {
   checkout scm
  }
  echo "${Build_Number}"
  def buildNo="${Build_Number}"
  echo "${WORKSPACE}"
  echo "${BRANCH_NAME}"
  def branchName="${BRANCH_NAME}"
  
  def msbuildPath =  tool name: 'MSBuild', type: 'msbuild'
  def msbuild = "${msbuildPath}\\MSBuild.exe"
  
  

  
  }
