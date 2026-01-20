# Jenkins Webhook Setup

## GitHub Webhook Configuration
1. Go to GitHub → Settings → Webhooks
2. Add webhook: `http://your-jenkins-server:8080/github-webhook/`
3. Content type: `application/json`
4. Events: Push, Pull Request

## Jenkins Configuration
- Pipeline triggers on: push to main, develop, staging
- Jenkinsfile location: `ci-cd/jenkins/Jenkinsfile`
