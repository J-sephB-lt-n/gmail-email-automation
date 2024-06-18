# gmail-email-automation

!!! I've given up on this project, because the gmail API seems not well-suited for non-consumer-facing applications !!!

The refresh token expires every 7 days in "testing" mode, and I don't feel like paying extra for Google Workspace, and waiting for google to validate my "app"

- Create a gmail account

- Set up python

```bash
python -m venv venv
source venv/bin/activate
pip install google-cloud-pubsub # tested on pip install google-cloud-pubsub==2.21.3
```

on GCP:

1. Enable pub/sub API

2. Enable Gmail API

3. Create an OAuth client ID (I used the gmail API in the google cloud website)

- this will require you to go through the consent screen setup

- I set the application type to 'desktop app' (this allows the user authorisation via a python script run on a laptop)
