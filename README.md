# Actions

Testing out github actions + webhooks


# Execute webhook_job via Rest API


``` curl -X POST \
  -H "Accept: application/vnd.github.v3+json" \
  -H "Authorization: token TOKEN" \
  https://api.github.com/repos/bjartekh/actions/actions/workflows/test-workflow.yml/dispatches \
  -d '{"ref":"main", "inputs":{"run_forrest":"true", "input1":"value1" }}'
```