node{
  stage('SCM checkout'){    
    git 'https://github.com/yogi40911/my-app'
  }
  stage('Build package'){
   // def mavenhome=tool name: 'Maven3', type: 'maven'
   // sh "${mavenhome}/bin/mvn package"  
    sh 'mvn package'
  }
}
