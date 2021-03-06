# Actions, resources, and condition keys for Amazon SimpleDB<a name="list_amazonsimpledb"></a>

**Tip**  
This page is moving to a new location on November 16, 2020\. Please update your bookmark to use the new page at [https://docs\.aws\.amazon\.com/service\-authorization/latest/reference/list\_amazonsimpledb\.html](https://docs.aws.amazon.com/service-authorization/latest/reference/list_amazonsimpledb.html)\. 

Amazon SimpleDB \(service prefix: `sdb`\) provides the following service\-specific resources, actions, and condition context keys for use in IAM permission policies\.

References:
+ Learn how to [configure this service](https://docs.aws.amazon.com/AmazonSimpleDB/latest/DeveloperGuide/)\.
+ View a list of the [API operations available for this service](https://docs.aws.amazon.com/AmazonSimpleDB/latest/DeveloperGuide/)\.
+ Learn how to secure this service and its resources by [using IAM](https://docs.aws.amazon.com/AmazonSimpleDB/latest/DeveloperGuide/UsingIAMWithSDB.html) permission policies\.

**Topics**
+ [Actions defined by Amazon SimpleDB](#amazonsimpledb-actions-as-permissions)
+ [Resource types defined by Amazon SimpleDB](#amazonsimpledb-resources-for-iam-policies)
+ [Condition keys for Amazon SimpleDB](#amazonsimpledb-policy-keys)

## Actions defined by Amazon SimpleDB<a name="amazonsimpledb-actions-as-permissions"></a>

You can specify the following actions in the `Action` element of an IAM policy statement\. Use policies to grant permissions to perform an operation in AWS\. When you use an action in a policy, you usually allow or deny access to the API operation or CLI command with the same name\. However, in some cases, a single action controls access to more than one operation\. Alternatively, some operations require several different actions\.

The **Resource types** column indicates whether each action supports resource\-level permissions\. If there is no value for this column, you must specify all resources \("\*"\) in the `Resource` element of your policy statement\. If the column includes a resource type, then you can specify an ARN of that type in a statement with that action\. Required resources are indicated in the table with an asterisk \(\*\)\. If you specify a resource\-level permission ARN in a statement using this action, then it must be of this type\. Some actions support multiple resource types\. If the resource type is optional \(not indicated as required\), then you can choose to use one but not the other\.

For details about the columns in the following table, see [The actions table](reference_policies_actions-resources-contextkeys.md#actions_table)\.


****  

| Actions | Description | Access level | Resource types \(\*required\) | Condition keys | Dependent actions | 
| --- | --- | --- | --- | --- | --- | 
|   [ BatchDeleteAttributes ](https://docs.aws.amazon.com/AmazonSimpleDB/latest/DeveloperGuide/API_BatchDeleteAttributes.html)  | Performs multiple DeleteAttributes operations in a single call, which reduces round trips and latencies\. | Write |   [ domain\* ](#amazonsimpledb-domain)   |  |  | 
|   [ BatchPutAttributes ](https://docs.aws.amazon.com/AmazonSimpleDB/latest/DeveloperGuide/API_BatchPutAttributes.html)  | With the BatchPutAttributes operation, you can perform multiple PutAttribute operations in a single call\. With the BatchPutAttributes operation, you can perform multiple PutAttribute operations in a single call\. | Write |   [ domain\* ](#amazonsimpledb-domain)   |  |  | 
|   [ CreateDomain ](https://docs.aws.amazon.com/AmazonSimpleDB/latest/DeveloperGuide/API_CreateDomain.html)  | The CreateDomain operation creates a new domain\. | Write |   [ domain\* ](#amazonsimpledb-domain)   |  |  | 
|   [ DeleteAttributes ](https://docs.aws.amazon.com/AmazonSimpleDB/latest/DeveloperGuide/API_DeleteAttributes.html)  | Deletes one or more attributes associated with the item\. | Write |   [ domain\* ](#amazonsimpledb-domain)   |  |  | 
|   [ DeleteDomain ](https://docs.aws.amazon.com/AmazonSimpleDB/latest/DeveloperGuide/API_DeleteDomain.html)  | The DeleteDomain operation deletes a domain\. | Write |   [ domain\* ](#amazonsimpledb-domain)   |  |  | 
|   [ DomainMetadata ](https://docs.aws.amazon.com/AmazonSimpleDB/latest/DeveloperGuide/API_DomainMetadata.html)  | Returns information about the domain, including when the domain was created, the number of items and attributes, and the size of attribute names and values\. | Read |   [ domain\* ](#amazonsimpledb-domain)   |  |  | 
|   [ GetAttributes ](https://docs.aws.amazon.com/AmazonSimpleDB/latest/DeveloperGuide/API_GetAttributes.html)  | Returns all of the attributes associated with the item\. | Read |   [ domain\* ](#amazonsimpledb-domain)   |  |  | 
|   [ ListDomains ](https://docs.aws.amazon.com/AmazonSimpleDB/latest/DeveloperGuide/API_ListDomains.html)  | Description for ListDomains | List |  |  |  | 
|   [ PutAttributes ](https://docs.aws.amazon.com/AmazonSimpleDB/latest/DeveloperGuide/API_PutAttributes.html)  | The PutAttributes operation creates or replaces attributes in an item\. | Write |   [ domain\* ](#amazonsimpledb-domain)   |  |  | 
|   [ Select ](https://docs.aws.amazon.com/AmazonSimpleDB/latest/DeveloperGuide/API_Select.html)  | Description for Select | Read |   [ domain\* ](#amazonsimpledb-domain)   |  |  | 

## Resource types defined by Amazon SimpleDB<a name="amazonsimpledb-resources-for-iam-policies"></a>

The following resource types are defined by this service and can be used in the `Resource` element of IAM permission policy statements\. Each action in the [Actions table](#amazonsimpledb-actions-as-permissions) identifies the resource types that can be specified with that action\. A resource type can also define which condition keys you can include in a policy\. These keys are displayed in the last column of the table\. For details about the columns in the following table, see [The resource types table](reference_policies_actions-resources-contextkeys.md#resources_table)\.


****  

| Resource types | ARN | Condition keys | 
| --- | --- | --- | 
|   [ domain ](https://docs.aws.amazon.com/sdb/latest/APIReference/DataModel.html)  |  arn:$\{Partition\}:sdb:$\{Region\}:$\{Account\}:domain/$\{DomainName\}  |  | 

## Condition keys for Amazon SimpleDB<a name="amazonsimpledb-policy-keys"></a>

SimpleDB has no service\-specific context keys that can be used in the `Condition` element of policy statements\. For the list of the global context keys that are available to all services, see [Available keys for conditions](reference_policies_condition-keys.html#AvailableKeys)\.