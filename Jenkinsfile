pipeline {
    agent { label 'DEV'}
    // tools {
    //     dockertool 'docker'
    // }
    // parameters {
    //     string(name: 'NAME', description: 'whats your name?')
    //     text(name: 'DESC', description: 'Describe about the job details')
    //     booleanParam(name: 'SKIP_TEST', description: 'want to skip running test cases?')
    //     choice(name: 'BRANCH', choices: ['master', 'dev'], description: 'choose branch')
    //     password(name: 'SONAR_SERVER_PWD', description: 'Enter Sonar password')
    // }
    environment {
        MY_CRED = credentials('jenkins')
    }
    stages {
        // specify various stages

    //    stage('Printing Parameters') {
    //        steps {
            //    echo "Hello ${params.NAME}"
            //    echo "Job Details: ${params.DESC}"
            //    echo "Skip running test cases?: ${params.SKIP_TEST}"
            //    echo "Branch choice: ${params.BRANCH}"
            //    echo "Sonar Password: ${params.SONAR_SERVER_PWD}"
                // script {
                //     def name = "${params.NAME}"
                //     def branch = "${params.BRANCH}"
                //     if (branch == 'master') {
                //         echo "Mr. ${name}"
                //     }
                //     else {
                //         echo "branch: ${branch}"
                //     }
                // }

            stage('Load credentials') {
                steps {
                    echo "username: ${MY_CRED_USR}"
                    echo "password: ${MY_CRED_PSW}"
                }
            }
    //        }
    //    }

        // stage1
        // stage('build'){
        //     steps {
        //      echo 'This is build phase....' 
        //      }
        // }

        // stage('test'){
        //     steps {
        //     echo 'This is test phase....'
        //     }
        // }
        // stage ('deploy'){
        //     steps {
        //         echo 'This is deployment phase....'
        //     }
        // }
    }
}
