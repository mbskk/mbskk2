pipeline{
  agent any
  stages{
    stage('Build'){
      steps{
        echo "Example build"
      }
    }
    stage('Deploy'){
      when{
        branch 'main'
        environment name:'branch', value:'main'
      }
      steps{
        echo "Deploy to main"
      }
    }
  }
}
