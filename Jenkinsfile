#!groovy
pipeline {
  agent any

  stages {
    stage('Trigger each snapshot and then release') {
      steps {
        script {
          pulp_yml = readYaml (file: 'sample.yaml')
          pulp_filters = pulp_yml.pulp_cron_config
        }
      }
    }
  }
}
