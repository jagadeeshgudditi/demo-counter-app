pipeline{
  stages{
    stage("Git checkout"){
      step{
        git branch: 'main', credentialsId: 'f04169fc-9b40-429d-a2ee-041ef3969cb3', url: 'https://github.com/jagadeeshgudditi/demo-counter-app.git'
      }
    }
  }
}
