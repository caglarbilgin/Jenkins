node{
  stage('SCM Checkout'){
    
    git 'https://github.com/caglarbilgin/Jenkins'
  }
  stage('Compile-Package'){
    def mvnHome = tool name: 'maven_3_6_0' , type: 'maven'
    sh "${mvnHome}/bin/mvn package"
  }
   stage('Publish test results') {
     steps{
       withMaven(maven : 'maven_3_6_0'){
         sh 'mvn test'
       }
     }
  }
}
