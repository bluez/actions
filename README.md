# GitHub Actions

This repository contains various GitHub Actions that are not appropriate to be
placed directly into the other repositories.

## Workflow list

Workflow files can be found from `.github/workflows/*`

### sync-repo.yml

This workflow synchronizes the bluez/bluez with upstream bluez tree.
Note that currently it does force-push to the bluez/bluez tree.
In order to change the checking duration, update the cron field.

```yaml
on:
  schedule:
    - cron: "*/30 * * * *"
```
