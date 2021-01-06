node{
  stage('SCM checkout'){    
    git 'https://github.com/yogi40911/my-app'
  }
stages {
        stage ('Compile Stage') {

            steps {
                withMaven(maven : 'maven_3_5_0') {
                    sh 'mvn clean compile'
                }
            }
        }
  stage('Build package'){
   // def mavenhome=tool name: 'Maven3', type: 'maven'
   // sh "${mavenhome}/bin/mvn package"  
    sh 'mvn package'
  }
}
