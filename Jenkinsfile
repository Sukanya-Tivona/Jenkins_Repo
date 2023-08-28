pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Build Backend') {
            steps {
                sh 'cd backend && npm install'
            }
        }
        stage('Build Frontend') {
            steps {
                sh 'cd frontend && npm install && npm run build'
            }
        }
        // stage('Deploy') {
        //     steps {
        //         sh './deploy-script.sh'  // Use a script to deploy your app
        //     }
        }
    }
//}






















//options>skipdefualtcheckout
// pipeline{

//     agent none//since we dont want to checkout the repo at pipeline level
    
//     stages{
    
//         stage('Build'){
//                    agent any
//                    options{
//                    skipDefaultCheckout()
//                    }
        
//                 steps{
                    
//                     echo "This Pipeline is working"
//                 }
//             }
//         }

// }


// pipeline{
//     agent any
    
//     stages{
    
//        stage('Build Master'){
//                        when {
//                           branch 'master'
//                             }
//         steps{
//             echo 'Building master'
//             }
//      }

//               stage('Build Dev'){
//                        when {
//                           branch 'Dev'
//                             }
//         steps{
//             echo 'Building Dev'
//             }
//      }
// }
//example 2
// node
// {
    
//   if(env.BRANCH_NAME =='master')
//     {
    
//        stage('Build Master'){
        
//             echo 'Building master'
//             }
//     }
//      if(env.BRANCH_NAME =='dev')
//     {
    
//        stage('Build DEV'){
        
//             echo 'Building dev'
//             }
//     }
// }
// node{
// 	properties(
// 		[
// 			overrideIndexTriggers(true)
// 		]
// 	)
	
// 	stage('Build'){
			
//                 echo 'Hello World'	
// 	}
// }
// node{
// stage("Build"){
// if(env.TAG_NAME !=null)
// {
// println("we r building a tag and tag is ${env.TAG_NAME}")
// }
// else{
// println("we r building a branch")
// }
// if(env.TAG_NAME == "releas-1.0")
// {
// println("we are building  release-1.0 tag")
// }
// }
// }
