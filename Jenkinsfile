node {
  stage 'st1'
    echo 'test1'
  stage 'st2'
    echo 'test2'
  stage 'build in development'
    kubernetes.pod('buildpod').withImage('maven').inside {   
      error 'hello world'
      git 'https://github.com/debianmaster/spring-sample-app.git'
      sh 'mvn clean install'
    } 
    echo 'asdfasdfs'
}