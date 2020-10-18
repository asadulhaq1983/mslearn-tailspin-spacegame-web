node(){
  stage("Checking Out Repo") {
   checkout scm
  }
  echo "${Build_Number}"
  echo "${WORKSPACE}"
  echo "${BRANCH_NAME}"
  stage("Zipping"){
    def b="${BRANCH_NAME}"
    if(b=='master')
       {
         zip zipFile:'Master'+${Build_Number}+'.zip', dir:'.'
  }
  else {
    zip zipFile:b+"_"+"${BuildNumber}"+.zip
  }
  
  }
}
