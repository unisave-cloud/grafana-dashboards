# Grafana Dashboards

This repository contains dashboards used in the internal Grafana monitoring tool. The repository is public so that it can be pulled easily by an init container.


## Editing dashboards

1. Create a new dashboard or download one and import
2. Set it up in grafana and save changes
3. Export via `Share > Export > View JSON > Copy To Clipboard`, do NOT export for external sharing, paste it into a JSON file in this repository
4. Make sure the filename and dashboard `"title"` are in sync (to not introduce mess)
5. Commit and push
6. Restart grafana to pull the latest commit `kubectl rollout restart deployment/grafana`
