pipeline {
  agent any
  parameters {
    string(name: 'USERNAME', defaultValue: 'guest', description: '사용자 이름')
    booleanParam(name: 'DEBUG_MODE', defaultValue: false, description: '디버그 모드 켜기')
    choice(name: 'ENV', choices: ['dev', 'staging', 'prod'], description: '배포 환경')
  }
  stages {
    stage('Example') {
      steps {
        echo "USERNAME=${params.USERNAME}"
        echo "DEBUG_MODE=${params.DEBUG_MODE}"
        echo "ENV=${params.ENV}"
      }
    }
  }
}
