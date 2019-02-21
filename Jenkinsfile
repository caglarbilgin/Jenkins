node{
  stage('SCM Checkout'){
    git 'https://github.com/caglarbilgin/Jenkins'
  }
  stage('Compile-Package'){
    sh 'mvn package'
  }
}
