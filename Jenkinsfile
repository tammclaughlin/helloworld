#!groovy

node {
  stage 'Checkout'
       checkut scm
  stage 'Setup'
       sh 'npm install'
  stage 'Mocha test'
       sh './node_modules/mocha/bin/mocha'
  stage 'Cleanup'
       echo 'prune and cleanup'
       sh 'npm prune'
       sh 'rm node_modules -rf'
}




