# Lab 4: ChatOps Integration

## Objective
Enable sharing by integrating CI/CD notifications into chat.

## Prerequisites
- Drone CI installed
- Slack/Teams webhook URL

## Steps
1. Configure Drone CI to send build notifications to Slack.
2. Add webhook in `.drone.yml`.
3. Trigger a build and observe notification.

## Commands
```yaml
notify:
  image: plugins/slack
  secrets: [ slack_webhook ]
  channel: devops-alerts
```
