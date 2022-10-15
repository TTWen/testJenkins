// 入门练习
// pipeline {
//     agent { any 'python:3.8' }
//     stages {
//         stage('build') {
//             steps {
//                 sh 'python --version'
//                 sh 'echo "Hello World"'
//                 sh '''
//                     echo "Multiline shell steps works too"
//                     ls -lah
//                 '''
//             }
//         }
//     }
// }
// 构建 python 应用
pipeline {
    agent { any 'python:3.8' }
    environment {
        Dhudson,plugins.git.GitSCM.ALLOW_LOCAL_CHECKOUT = 'true'
    }

    stages {
        stage('build') {
            steps {
//                 sh 'python --version'
                sh 'echo "Hello World"'
                sh '''
                    echo "Multiline shell steps works too"
                    ls -lah
                '''
            }
        }
    }
}