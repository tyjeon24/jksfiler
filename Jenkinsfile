pipeline {
  agent any
  parameters {
    choice(
      name: 'ENV',
      choices: ['dev', 'staging', 'prod'],
      description: '배포 환경을 선택하세요'
    )
    string(name: 'USERNAME', defaultValue: 'guest')
    booleanParam(name: 'DEBUG', defaultValue: false)
  }
  stages {
    stage('Print Params') {
      steps {
        echo "ENV=${params.ENV}"
        echo "USERNAME=${params.USERNAME}"
        echo "DEBUG=${params.DEBUG}"
      }
    }
  }
}
