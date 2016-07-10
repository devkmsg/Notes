## Parse json for private IP Addresses

```bash
aws ec2 describe-instances --filters 'Name=tag:Name,Values=service-1' | jq '.Reservations[].Instances[].PrivateIpAddress'
```
