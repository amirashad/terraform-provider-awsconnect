---
page_title: "awsconnect_instance Data Source - terraform-provider-awsconnect"
subcategory: ""
description: |-
  The awsconnect_instance data source allows you to retrieve information about Connect Instance.
---

# Data Source `awsconnect_instance`

The awsconnect_instance data source allows you to retrieve information about Connect Instance by it's InstanceId.

## Example Usage

```terraform
data "awsconnect_instance" "instance" {
  instance_id = "ebdfba29-ca78-41ea-b980-b328ab640a77"
}

```

## Attributes Reference

The following attributes are exported.

- `instance_id` - A InstanceId of Connect Instance. See [Instance](#instance) below for details.

### Instance

- `instance_id` -  The identifier of the Amazon Connect instance.
- `arn` - The AWS ARN of resource.
- `instance_alias` - The name for your instance.
- `identity_management_type` - The type of identity management for your Amazon Connect users.
- `inbound_calls_enabled` - Your contact center handles incoming calls.
- `outbound_calls_enabled` - Your contact center allows outbound calls.
