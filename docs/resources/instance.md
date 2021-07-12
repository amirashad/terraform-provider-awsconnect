---
page_title: "awsconnect_instance Resource - terraform-provider-awsconnect"
subcategory: ""
description: |-
  The awsconnect_instance resource allows you to configure a AWS Connect Instance.
---

# Resource `awsconnect_instance`

-> Visit the [Perform CRUD operations with Providers](https://learn.hashicorp.com/tutorials/terraform/provider-use?in=terraform/providers&utm_source=WEBSITE&utm_medium=WEB_IO&utm_offer=ARTICLE_PAGE&utm_content=DOCS) Learn tutorial for an interactive getting started experience.

The awsconnect_instance resource allows you to configure a AWS Connect Instance.

-> Visit the [AWS Connect CreateInstance API](https://docs.aws.amazon.com/connect/latest/APIReference/API_CreateInstance.html) for detailed API information
## Example Usage

```terraform
resource "awsconnect_instance" "second" {
  instance_alias           = "sample-instance"
  identity_management_type = "CONNECT_MANAGED"
  inbound_calls_enabled    = true
  outbound_calls_enabled   = true
}
```

## Argument Reference

- `instance_alias` - The name for your instance.
- `identity_management_type` - The type of identity management for your Amazon Connect users.
- `inbound_calls_enabled` - Your contact center handles incoming calls.
- `outbound_calls_enabled` - Your contact center allows outbound calls.
