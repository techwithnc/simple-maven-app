def mygvscript
def matcher
def version

pipeline {
    agent any
    // environment {
    //     IMAGE_NAME = ""
    // }
    tools{
        maven '01Maven'
    }
    stages{
        stage("Prepare"){
            steps{
                script{
                    mygvscript = load "script.groovy"
                }
            }
        }
        stage("Build_App"){
            steps{
                script{
                    mygvscript.buildApp()
                }
            }
        }
        // stage("Build_IMAGE"){
        //     steps {
        //         script {
        //             mygvscript.buildImage()
        //         }
        //     }
        // }
        // stage("Build_IMAGE"){
        //     steps {
        //         script {
        //             mygvscript.buildImage()
        //         }
        //     }
        // }  
        // stage("Push_IMAGE") {
        //     steps {
        //         script {
        //             mygvscript.pushImage()
        //         }
        //     }
        // }
    }
}
 