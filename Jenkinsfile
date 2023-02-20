pipeline{
  agent any
  stages{
    stage('Build'){
      steps{
        sh 'g++ -o task5 task5_code.cpp'
        build job: 'pratham.r_pes1ug20cs308-1'
      }
    }
    stage('Test'){
      steps{
        sh './task5'
       // sh 'exit 1' //error
      }
    }
   stage('Deploy'){
      steps{
        echo 'Deploying'
        
      }
    }
  }
  post{
    failure{
      echo 'Pipeline failed'
    }
  }
}
