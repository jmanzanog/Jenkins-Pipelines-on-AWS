pipeline{
    agent any
    stages {
        stage('Upload to AWS') {
            steps {
                withAWS(region:'ap-northeast-2', credentials:'1da5412b-e88c-449a-8a60-1505a44f5865'){
                    s3Upload(file:'index.html', bucket:'jmanzano-jenkins', path:'')
                }
            }
        }
    }
}
