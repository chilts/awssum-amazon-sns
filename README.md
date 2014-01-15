# awssum-amazon-sns #

This is an ```AwsSum``` plugin!

You'll need to add [awssum-amazon-sns](https://github.com/awssum/awssum-amazon-sns/) to your package.json
dependencies. Both [awssum](https://github.com/awssum/awssum/) and
[awssum-amazon](https://github.com/awssum/awssum-amazon/) are pulled in as peer dependencies.

## Example ##

List all your topics:

```
var fmt = require('fmt');
var amazonSns = require('awssum-amazon-sns');

var sns = new amazonSns.Sns({
    'accessKeyId'     : process.env.ACCESS_KEY_ID,
    'secretAccessKey' : process.env.SECRET_ACCESS_KEY,
    'region'          : amazonSns.US_EAST_1,
});

sns.ListTopics(function(err, data) {
    fmt.dump(err, 'err');
    fmt.dump(data, 'data');
});
```

## Operations ##

### AddPermission ###

Docs: [AddPermission on AWS](http://docs.amazonwebservices.com/sns/latest/api/API_AddPermission.html)

### ConfirmSubscription ###

Docs: [ConfirmSubscription on AWS](http://docs.amazonwebservices.com/sns/latest/api/API_ConfirmSubscription.html)

### CreateTopic ###

Docs: [CreateTopic on AWS](http://docs.amazonwebservices.com/sns/latest/api/API_CreateTopic.html)

### DeleteTopic ###

Docs: [DeleteTopic on AWS](http://docs.amazonwebservices.com/sns/latest/api/API_DeleteTopic.html)

### GetSubscriptionAttributes ###

Docs: [GetSubscriptionAttributes on AWS](http://docs.amazonwebservices.com/sns/latest/api/API_GetSubscriptionAttributes.html)

### GetTopicAttributes ###

Docs: [GetTopicAttributes on AWS](http://docs.amazonwebservices.com/sns/latest/api/API_GetTopicAttributes.html)

### ListSubscriptions ###

Docs: [ListSubscriptions on AWS](http://docs.amazonwebservices.com/sns/latest/api/API_ListSubscriptions.html)

### ListSubscriptionsByTopic ###

Docs: [ListSubscriptionsByTopic on AWS](http://docs.amazonwebservices.com/sns/latest/api/API_ListSubscriptionsByTopic.html)

### ListTopics ###

Docs: [ListTopics on AWS](http://docs.amazonwebservices.com/sns/latest/api/API_ListTopics.html)

### Publish ###

Docs: [Publish on AWS](http://docs.amazonwebservices.com/sns/latest/api/API_Publish.html)

### RemovePermission ###

Docs: [RemovePermission on AWS](http://docs.amazonwebservices.com/sns/latest/api/API_RemovePermission.html)

### SetSubscriptionAttributes ###

Docs: [SetSubscriptionAttributes on AWS](http://docs.amazonwebservices.com/sns/latest/api/API_SetSubscriptionAttributes.html)

### SetTopicAttributes ###

Docs: [SetTopicAttributes on AWS](http://docs.amazonwebservices.com/sns/latest/api/API_SetTopicAttributes.html)

### Subscribe ###

Docs: [Subscribe on AWS](http://docs.amazonwebservices.com/sns/latest/api/API_Subscribe.html)

### Unsubscribe ###

Docs: [Unsubscribe on AWS](http://docs.amazonwebservices.com/sns/latest/api/API_Unsubscribe.html)



# Author #

Written by [Andrew Chilton](http://chilts.org/) - [Blog](http://chilts.org/blog/) -
[Twitter](https://twitter.com/andychilton).

# License #

* [Copyright 2011-2013 Apps Attic Ltd.  All rights reserved.](http://appsattic.mit-license.org/2011/)
* [Copyright 2013 Andrew Chilton.  All rights reserved.](http://chilts.mit-license.org/2013/)

(Ends)
