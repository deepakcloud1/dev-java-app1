// pipeline{
//     agent any
//     stages{
//         stage('Git Checkout')
//             step{
//                 script{
//                     git branch: 'main', url: 'https://github.com/deepakcloud1/dev-java-app1.git'
//                 }
//             }
//     }
// }

pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                script {       
                    git branch: 'main', url: 'https://github.com/deepakcloud1/dev-java-app1.git'
                }
            }
        }           
    }
}
    
   