pipeline {
  agent any
  stages {
    stage('Build') { steps { echo 'Compile & package (eg:Maven/Gradle)' } }
    stage('Unit & Integration Tests') { steps { echo 'Run unit & integration tests (eg: JUnit/Mocha+Chai)' } }
    stage('Code Analysis') { steps { echo 'Static analysis (eg: SonarQube/SonarCloud/ESLint)' } }
    stage('Security Scan') { steps { echo 'Dependency/code scan (eg: npm audit/OWASP Dep-Check)' } }
    stage('Deploy to Staging') { steps { echo 'Deploy to staging (eg:AWS EC2/Docker/Ansible)' } }
    stage('Integration Tests on Staging') { steps { echo 'E2E tests on staging (eg:Selenium/Newman)' } }
    stage('Deploy to Production') { steps { echo 'Promote to production (eg: EC2/Kubernetes)' } }
  }
}
