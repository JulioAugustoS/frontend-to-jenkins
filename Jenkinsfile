node {
  def app_name = "frontend-to-jenkins"
  def git_url = "git@github.com:RafaelAugustoS/frontend-to-jenkins.git"

  stage('Clone Repository'){
    git branch: 'master',
    credentialsId: 'jenkins',
    url: git_url
  }

  stage('Build'){
    sh "cd .. && cp -r ${app_name}/* /var/www/html"
  }
}