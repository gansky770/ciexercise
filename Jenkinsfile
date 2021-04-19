node {
  stage ('Build Jar  ') {
    git url: 'https://github.com/gansky770/ciexercise.git'
    withMaven {
      sh "mvn clean verify"
    } // withMaven will discover the generated Maven artifacts, JUnit Surefire & FailSafe reports and FindBugs reports
  }

  stage ('Tests- Static code analysis') {
      
  }

  stage ('Build docker image & push to registry') {
      
  }
}