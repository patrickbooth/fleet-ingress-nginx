pipeline {
  agent any
  stages {
    stage('Checkout Source') {
      steps {
        git 'https://github.com/patrickbooth/fleet-ingress-nginx'
      }
    }
    stage('Deploying fleet gitrepo resource') {
      steps {
        script {
          kubernetesDeploy(configs: "./gitrepo/gitrepo.yaml")
        }
      }
    }
  }
}
