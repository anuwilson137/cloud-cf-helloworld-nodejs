@Library('piper-lib-os') _
pipeline {
    agent { label 'master' }
    stages {
        stage('prepare') {
          checkout scm
          setupCommonPipelineEnvironment script:this
        }
        stage('build') {
          mtaBuild script: this
        }
    }
}
