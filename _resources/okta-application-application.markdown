---
layout: publisher
name: "Okta::Application::Application"
description: Okta Resource
publisher: "Okta"
---

## Regions
<select>
    <option>US-EAST-1</option>
    <option>US-EAST-2</option>
</select>

<h2>Versions</h2>
<p>I think we ignore this...</p>


# okta-application-application

## Description

Manage an Application in Okta.

## References

* [Documentation](https://github.com/aws-ia/cloudformation-okta-resource-providers)
* [Source](https://github.com/aws-ia/cloudformation-okta-resource-providers.git)

## Usage

In order to use this library, you will need to activate this AWS CloudFormation Registry type in your account. You can do this via the AWS Management Console or using the [AWS CLI](https://aws.amazon.com/cli/) using the following command:

```sh
aws cloudformation activate-type \
  --type-name Okta::Application::Application \
  --publisher-id c830e97710da0c9954d80ba8df021e5439e7134b \
  --type RESOURCE \
  --execution-role-arn ROLE-ARN
```

Alternatively:

```sh
aws cloudformation activate-type \
  --public-type-arn arn:aws:cloudformation:us-east-1::type/resource/c830e97710da0c9954d80ba8df021e5439e7134b/Okta-Application-Application \
  --execution-role-arn ROLE-ARN
```

You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).

## Feedback

This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation] project based on the API schema published for `Okta::Application::Application`.

* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fokta-application-application+v1.2.0).
* Issues related to `Okta::Application::Application` should be reported to the [publisher](https://github.com/aws-ia/cloudformation-okta-resource-providers).

[cdklabs/cdk-cloudformation]: https://github.com/cdklabs/cdk-cloudformation

## License

Distributed under the Apache-2.0 License.