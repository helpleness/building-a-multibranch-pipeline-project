pipeline {
    // ʹ��һ������ Node.js 18 �� Docker ������Ϊ��������
    agent {
        docker { image 'node:18-alpine' }
    }
    stages {
        stage('Build') {
            steps {
                // ����������npm ����Ϳ��Ա��ҵ���
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
