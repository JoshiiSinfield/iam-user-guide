# Actions, resources, and condition keys for Amazon Storage Gateway<a name="list_amazonstoragegateway"></a>

**Tip**  
This page is moving to a new location on November 16, 2020\. Please update your bookmark to use the new page at [https://docs\.aws\.amazon\.com/service\-authorization/latest/reference/list\_amazonstoragegateway\.html](https://docs.aws.amazon.com/service-authorization/latest/reference/list_amazonstoragegateway.html)\. 

Amazon Storage Gateway \(service prefix: `storagegateway`\) provides the following service\-specific resources, actions, and condition context keys for use in IAM permission policies\.

References:
+ Learn how to [configure this service](https://docs.aws.amazon.com/storagegateway/latest/userguide/)\.
+ View a list of the [API operations available for this service](https://docs.aws.amazon.com/storagegateway/latest/APIReference/)\.
+ Learn how to secure this service and its resources by [using IAM](https://docs.aws.amazon.com/storagegateway/latest/userguide/UsingIAMWithStorageGateway.html) permission policies\.

**Topics**
+ [Actions defined by Amazon Storage Gateway](#amazonstoragegateway-actions-as-permissions)
+ [Resource types defined by Amazon Storage Gateway](#amazonstoragegateway-resources-for-iam-policies)
+ [Condition keys for Amazon Storage Gateway](#amazonstoragegateway-policy-keys)

## Actions defined by Amazon Storage Gateway<a name="amazonstoragegateway-actions-as-permissions"></a>

You can specify the following actions in the `Action` element of an IAM policy statement\. Use policies to grant permissions to perform an operation in AWS\. When you use an action in a policy, you usually allow or deny access to the API operation or CLI command with the same name\. However, in some cases, a single action controls access to more than one operation\. Alternatively, some operations require several different actions\.

The **Resource types** column indicates whether each action supports resource\-level permissions\. If there is no value for this column, you must specify all resources \("\*"\) in the `Resource` element of your policy statement\. If the column includes a resource type, then you can specify an ARN of that type in a statement with that action\. Required resources are indicated in the table with an asterisk \(\*\)\. If you specify a resource\-level permission ARN in a statement using this action, then it must be of this type\. Some actions support multiple resource types\. If the resource type is optional \(not indicated as required\), then you can choose to use one but not the other\.

For details about the columns in the following table, see [The actions table](reference_policies_actions-resources-contextkeys.md#actions_table)\.


****  
[\[See the AWS documentation website for more details\]](http://docs.aws.amazon.com/IAM/latest/UserGuide/list_amazonstoragegateway.html)

## Resource types defined by Amazon Storage Gateway<a name="amazonstoragegateway-resources-for-iam-policies"></a>

The following resource types are defined by this service and can be used in the `Resource` element of IAM permission policy statements\. Each action in the [Actions table](#amazonstoragegateway-actions-as-permissions) identifies the resource types that can be specified with that action\. A resource type can also define which condition keys you can include in a policy\. These keys are displayed in the last column of the table\. For details about the columns in the following table, see [The resource types table](reference_policies_actions-resources-contextkeys.md#resources_table)\.


****  

| Resource types | ARN | Condition keys | 
| --- | --- | --- | 
|   [ device ](https://docs.aws.amazon.com/storagegateway/latest/userguide/resource_vtl-devices.html)  |  arn:$\{Partition\}:storagegateway:$\{Region\}:$\{Account\}:gateway/$\{GatewayId\}/device/$\{Vtldevice\}  |  | 
|   [ gateway ](https://docs.aws.amazon.com/storagegateway/latest/userguide/StorageGatewayConcepts.html)  |  arn:$\{Partition\}:storagegateway:$\{Region\}:$\{Account\}:gateway/$\{GatewayId\}  |   [ aws:ResourceTag/$\{TagKey\} ](#amazonstoragegateway-aws_ResourceTag___TagKey_)   | 
|   [ share ](https://docs.aws.amazon.com/storagegateway/latest/userguide/GettingStartedCreateFileShare.html)  |  arn:$\{Partition\}:storagegateway:$\{Region\}:$\{Account\}:share/$\{ShareId\}  |   [ aws:ResourceTag/$\{TagKey\} ](#amazonstoragegateway-aws_ResourceTag___TagKey_)   | 
|   [ tape ](https://docs.aws.amazon.com/storagegateway/latest/userguide/StorageGatewayConcepts.html#storage-gateway-vtl-concepts)  |  arn:$\{Partition\}:storagegateway:$\{Region\}:$\{Account\}:tape/$\{TapeBarcode\}  |   [ aws:ResourceTag/$\{TagKey\} ](#amazonstoragegateway-aws_ResourceTag___TagKey_)   | 
|   [ tapepool ](https://docs.aws.amazon.com/storagegateway/latest/userguide/CreatingCustomTapePool.html)  |  arn:$\{Partition\}:storagegateway:$\{Region\}:$\{Account\}:tapepool/$\{PoolId\}  |   [ aws:ResourceTag/$\{TagKey\} ](#amazonstoragegateway-aws_ResourceTag___TagKey_)   | 
|   [ target ](https://docs.aws.amazon.com/storagegateway/latest/userguide/GettingStartedCreateVolumes.html)  |  arn:$\{Partition\}:storagegateway:$\{Region\}:$\{Account\}:gateway/$\{GatewayId\}/target/$\{IscsiTarget\}  |  | 
|   [ volume ](https://docs.aws.amazon.com/storagegateway/latest/userguide/StorageGatewayConcepts.html#volume-gateway-concepts)  |  arn:$\{Partition\}:storagegateway:$\{Region\}:$\{Account\}:gateway/$\{GatewayId\}/volume/$\{VolumeId\}  |   [ aws:ResourceTag/$\{TagKey\} ](#amazonstoragegateway-aws_ResourceTag___TagKey_)   | 

## Condition keys for Amazon Storage Gateway<a name="amazonstoragegateway-policy-keys"></a>

Amazon Storage Gateway defines the following condition keys that can be used in the `Condition` element of an IAM policy\. You can use these keys to further refine the conditions under which the policy statement applies\. For details about the columns in the following table, see [The condition keys table](reference_policies_actions-resources-contextkeys.md#context_keys_table)\.

To view the global condition keys that are available to all services, see [Available global condition keys](reference_policies_condition-keys.html#AvailableKeys)\.


****  

| Condition keys | Description | Type | 
| --- | --- | --- | 
|   aws:RequestTag/$\{TagKey\}  | Filters acess based on the allowed set of values for each of the tags | String | 
|   aws:ResourceTag/$\{TagKey\}  | Filters acess based on tag\-value associated with the resource | String | 
|   aws:TagKeys  | Filters acess based on the presence of mandatory tags in the request | String | 