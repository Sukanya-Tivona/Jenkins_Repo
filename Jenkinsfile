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
node{
	properties(
		[
			overrideIndexTriggers(true)
		]
	)
	
	stage('Build'){
			
                echo 'Hello World'	
	}
}
