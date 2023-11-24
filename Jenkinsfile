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
                // Clean workspace before checkout (optional)
                deleteDir()

                // Checkout code from the Git repository
                script {
                    // Replace 'your-repository-url' with the actual URL of your Git repository
                    git branch: 'main', url: 'https://github.com/deepakcloud1/dev-java-app1.git'
                }
            }
        }
        
        // Add more stages as needed for your build, test, deploy, etc.
    }
    
    post {
        success {
            echo 'Git checkout successful'
        }
        failure {
            echo 'Git checkout failed'
        }
    }
}
