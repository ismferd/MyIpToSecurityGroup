# MyIpToSecurityGroup
Add myIP to segurity group for AWS account

#USE
This script add your IP to SG that you like choose.
You need the credentials "aws_access_key_id" and "aws_secret_access_key" into $HOME/.aws/config

#LAUNCH
For run launch:
example:

File config:
  $HOME/.aws/config:
  [profile environment-pro]
  output = table
  region = eu-west-1
  aws_access_key_id = XXXXXX
  aws_secret_access_key = xxxxx

#RUN
  Run only with environment:
  python myIpToSecurityGroup.py "environment-dev"
You see all SG about yout account
  python myIpToSecurityGroup.py "environment-dev" default
You add your IP to SG default
