// Define the variables
def dockerPublisherName = "rahulraju"
def dockerRepoName = "sample-ng-app"

def gitRepoName = "https://github.com/lRAHULl/dynamic-branch-jenkins.git"
//def gitBranch = sh(returnStdout: true, script: 'git rev-parse --abbrev-ref HEAD').trim()

def customLocalImage = "sample-ng-app-image"

properties([pipelineTriggers([githubPush()])])
pipeline {
    agent {
        node {
            label 'linux-slave'
        }
    }

    stages {
        stage('Checkout') {
            steps {
            sh'printenv'
        echo "${scm}"

                git url: "${gitRepoName}", branch:"**"
            }
        }

    }
}
