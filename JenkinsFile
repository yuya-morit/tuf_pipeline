pipeline {
    agent any
    stages {
        stage('ビルド') {
            steps {
                echo 'Start build'
            }
        }
        stage('テスト') {
            steps {
                writeFile encoding: 'UTF-8', file: 'out.txt', text: 'testtest'
            }
        }
        stage('リリース') {
            steps {
                input "実行しますか？"
                echo '完了'
            }
        }
    }
}
