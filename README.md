# Exam Action Event


## Schedule

```yaml
name: Exam cron
on:
  schedule:
    - cron: "*/5 * * * *"
jobs:
  echo:
    runs-on: ubuntu-latest
    steps:
      - name: Log github
        run: echo "$GITHUB"
        env:
          GITHUB: ${{ toJson(github) }}
```

```json
{
  "token": "***",
  "ref": "refs/heads/master",
  "sha": "26b1e90af55362d2e89c3f9182f9eaeebc457f52",
  "repository": "marocchino/exam-action-event",
  "repositoryUrl": "git://github.com/marocchino/exam-action-event.git",
  "run_id": "52820551",
  "run_number": "1",
  "actor": "marocchino",
  "workflow": "Exam cron",
  "head_ref": "",
  "base_ref": "",
  "event_name": "schedule",
  "event": {
    "schedule": "*/5 * * * *"
  },
  "workspace": "/home/runner/work/exam-action-event/exam-action-event",
  "action": "run"
}
```
