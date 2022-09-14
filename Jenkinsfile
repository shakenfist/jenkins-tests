#!groovy
pipeline {
  agent any

  stages {
    stage('Test 2') {
      steps {
        script {
          pulp_yml = readYaml (file: 'sample.yaml')
          pulp_filters = pulp_yml.pulp_cron_config
        }
      }
    }
  }
}
