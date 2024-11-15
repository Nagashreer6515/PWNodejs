pipeline{
agent any
 stages{
  stage('Pulling code from git'){
    steps{
        git 'https://github.com/Nagashreer6515/PWNodejs.git'
    }
}
    stage("Installing npm dependencies"){
     steps{
        bat 'npm install'
    }
}
    stage('Installing playwright dependencies'){
    steps{
        bat 'npx playwright install'
    }
}
    stage('Building jonb in headed mode'){
    steps{
        bat 'npx playwright test'
    }
}
}
}
