# docker-selenium-lambda

![badge](https://github.com/umihico/docker-selenium-lambda/actions/workflows/demo-test.yml/badge.svg)
![badge](https://github.com/umihico/docker-selenium-lambda/actions/workflows/auto-update.yml/badge.svg)

> :warning: **Caution!**
>
> Updating Chromium and Chromedriver versions to v115 or later is postponed in this repository. I'll try to fix later.
> See https://chromedriver.chromium.org/downloads

This is minimum demo of headless chrome and selenium on container image on AWS Lambda

This image goes with these versions. [These are automatically updated and tested everyday.](https://github.com/umihico/docker-selenium-lambda/actions)

- Python 3.11.5
- chromium 114.0.5735.0
- chromedriver 114.0.5735.90
- selenium 4.13.0

## Running the demo

```bash
$ npm install -g serverless # skip this line if you have already installed Serverless Framework
$ sls create --template-url "https://github.com/umihico/docker-selenium-lambda/tree/main" --path docker-selenium-lambda && cd $_
$ sls deploy
$ sls invoke --function demo # Yay! You will get texts of example.com
```

Available tags are listed [here](https://hub.docker.com/r/umihico/aws-lambda-selenium-python/tags)