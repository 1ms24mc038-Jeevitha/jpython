pipeline{
   agent any
   tools{
     jdk 'jdk21'
     }
     stages{
        stage('checkout'){
        steps{
        git branch:"main",url:" "
        }
    }
    stage('java compile'){
      steps{
          echo'compiling java file'
          sh'javac
