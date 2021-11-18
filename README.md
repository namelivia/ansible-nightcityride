# NightCityRide Ansible role

## This is a WIP

The project depends on the collection `community.docker` but apparently this [cannot be listed as a dependency](https://github.com/ansible/ansible/issues/62847) so make sure you add it to your `requirements.yml` file like:

```yml
---

collections:
  - community.docker

roles:
  - src: https://github.com/namelivia/ansible-nightcityride
```

## Required variables
 - `cloudwatch_region` Cloudwatch region to send the logs to.
 - `cloudwatch_log_group` Cloudwatch log group to send the logs to.
 - `domain_name` The domain name in which the app will be served from.
 - `backup_day` Day of the week in which the content will be backed up.
 - `consumer_key`: Consumer key for the Twitter API.
 - `consumer_secret`: Consumer secret for the Twitter API.
 - `access_token_key`: Access token key for the Twitter API.
 - `access_token_secret`: Access token secret for the Twitter API.
