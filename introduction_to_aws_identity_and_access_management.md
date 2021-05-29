- IAM users takes care of the authentication
[link text](#abcd)
- To take care authorization you can attach an IAM policy to a user in order
to grant or deny permissions
- Actions: are AWS api calls
- IAM policies are JSON based  documents

## IAM policy
> Contains permissions that allow the identity to which it's attached to perform any EC2 related action 
```js
{
 "Statement": [{
    "Effect": "Allow", //Allow|Deny
    "Action": "ec2:*",//AWS api call, restrict to specific api calls section 1.0
    "Resource": <Amazon-Resource-Name-Here>//Allows you to restrict which AWS resources the actions are allowed to be performed against
    "Condition": {
       <Condition-Here>//Can further restrict actions
    }
   
 }]
}

```


### Section 1.0
> Any user with this policy attached would be able to run EC2 instances but perform no other EC2 related tasks
`Action: "ec2:RunInstances"`

## Identity
Users or groups

### <a name="abcd"></a>hjkhkjsdfgh