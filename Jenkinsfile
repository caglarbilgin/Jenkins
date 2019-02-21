node{
  stage('SCM Checkout'){
    
    git 'https://github.com/caglarbilgin/Jenkins'
  }
  stage('Compile-Package'){
    def mvnHome = tool name: 'apache-maven-3.6.0' , type: 'maven'
    sh "${mvnHome}/bin/mvn package"
  }
}
