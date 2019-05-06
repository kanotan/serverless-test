# introduction

This is tutorial of AWS Lambda for ruby with serverless framework. 

# install

npm install -g serverless

# initialize

serverless create --template aws-ruby --name [project-name] --path [project-path]

# run local

- serverless invoke local --function hello
- sls invoke local --function hello

Both command able to use "serverless" and "sls".

# setting credential

sls config credentials --provider aws --key [aws-key] --secret [aws-secret] --profile [profile-name]

# deploy

sls deploy --aws-profile [profile-name]

# run online

sls invoke --function hello --aws-profile [profile-name]

# run on browser

After setting of API Gateway, this program can run on browser.

https://xxxxxxx.execute-api.ap-northeast-1.amazonaws.com/dev/kanotan-serverless/hello

# remove

sls remove --aws-profile [profile-name]
