# aws-multi-account-management

## Deployment

### AWS-Config
Launch Config CF template via AWS Console or CLI

```
# Deploy stack
aws cloudformation create-stack \
--stack-name <stack-name> \
--template-body file://aws-config-aggregator.yml \
--on-failure DO_NOTHING \
--region <region> \
--capabilities CAPABILITY_NAMED_IAM 

# Delete stack
aws cloudformation delete-stack \
--stack-name <stack-name> \
--region <region>
```