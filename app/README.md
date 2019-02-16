# OpenUnison Simple Quickstart

This quickstart will create simple OpenUnison deployment that will authenticate
a static user defined using environment variables.  Its meant to be a starting
point for learning how to build and deploy OpenUnison.

## Environment Variables

| Variable | Description | Example |
| -------- | ----------- | ------- |
| OU_HOST | The host name users will use to access the site | myapp.mycompany.lan |
| TEST_USER_NAME | The name of the test user | testuser |
| TEST_USER_PASSWORD | The password for the test user | secret |
| unisonKeystorePassword | Password for the OpenUnison keystore |
| unisonKeystorePath | The path to OpenUnison's keystore |

## Use

Once deployed, access this site by navigating to https://OU_HOST/ replacing
OU_HOST with the value of the OU_HOST environment variable.  For instance, if
OU_HOST is myapp.mycompany.lan use https://myapp.mycompany.lan/.  Once prompoted
for a username and password, use the values specified for TEST_USER_NAME and
TEST_USER_PASSWORD respectively.  Once logged in, a page showing all headers,
request and session variables is shown.
