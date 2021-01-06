node{
  stage('SCM checkout'){
    
    git 'https://github.com/yogi40911/Spring-MongoKubernatesEample/new/'
  }
  stage('Build package'){
    def mavenhome=tool name: 'Maven3', type: 'maven'
    sh "${mavenhome}/bin/mvn package"    
  }
}
