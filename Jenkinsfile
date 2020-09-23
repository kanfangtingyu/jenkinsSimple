// pipeline {
//     // agent 指示 Jenkins 为整个流水线分配一个执行器（在 Jenkins 环境中的任何可用代理/节点上）和工作区。
//     agent any
//     stages {
//         stage('Build') {
//             steps {
//                 //echo 写一个简单的字符串到控制台输出
//                 sh 'echo "Hello world!"'
//             }
//         }
//     }
// }

pipeline {
    agent {
        docker { image 'node:7-alpine' }
    }
    stages {
        stage('Test') {
            steps {
                sh 'node --version'
            }
        }
    }
}