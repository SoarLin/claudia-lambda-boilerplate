# Lambda Boilerplate

## Before Usage

* make sure your node **version > 8.0**
* change package.json info for your lambda function
  * name
  * description
  * author

```
{
  "name": "claudia-lambda-boilerplate",
  "description": "Use claudia.js deploy lambda function boilerplate",
  "author": "Soar <soar.lin@gmail.com>",
}
```

* edit package.json config to meet your needs
* default
  * aws region is `ap-northeast-1`
  * lambda use memory is `128MB`
  * lambda timeout is `5 sec.`

```
  "config": {
    "profile": "default",
    "region": "ap-northeast-1",
    "memory": "128",
    "timeout": "5"
  }
```

## Add your role policies

Your can add aws policies for lambda function executor at `policies/lambda-basic-policy.json` or edit at AWS IAM console

## Usage

* lauch project to AWS lambda

```
npm run deploy
```

* update lambda

```
npm run update
```