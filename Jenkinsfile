pipeline {
  agent any
  triggers { pollSCM('H/2 * * * *') } // check repo every 2 mins

  stages {
    stage('Stage 1: Build') {
      steps {
        echo 'Task: Compile & package code'
        echo 'Tool: Maven (or Gradle/npm)'
      }
    }
    stage('Stage 2: Unit & Integration Tests') {
      steps {
        echo 'Task: Run unit + integration tests'
        echo 'Tools: JUnit/TestNG (Java) or Mocha/Jest (JS)'
      }
    }
    stage('Stage 3: Code Analysis') {
      steps {
        echo 'Task: Static code analysis'
        echo 'Tools: SonarQube/SonarCloud, ESLint/PMD'
      }
    }
    stage('Stage 4: Security Scan') {
      steps {
        echo 'Task: Scan for vulnerabilities'
        echo 'Tools: OWASP Dependency-Check, npm audit, Snyk'
      }
    }
    stage('Stage 5: Deploy to Staging') {
      steps {
        echo 'Task: Deploy to staging server'
        echo 'Tool: AWS EC2, Docker, Ansible'
      }
    }
    stage('Stage 6: Integration Tests on Staging') {
      steps {
        echo 'Task: Run integration tests in staging'
        echo 'Tools: Postman/Newman, Selenium'
      }
    }
    stage('Stage 7: Deploy to Production') {
      steps {
        echo 'Task: Deploy to production server'
        echo 'Tool: AWS EC2, Docker, Ansible'
      }
    }
  }
}
