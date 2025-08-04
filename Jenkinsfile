pipeline {
    // 使用一个包含 Node.js 18 的 Docker 容器作为构建环境
    agent {
        docker { image 'node:18-alpine' }
    }
    stages {
        stage('Build') {
            steps {
                // 在这个环境里，npm 命令就可以被找到了
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                sh 'npm test'
            }
        }
    }
}
