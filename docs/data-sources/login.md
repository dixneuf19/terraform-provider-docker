---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "docker_login Data Source - docker"
subcategory: ""
description: |-
  Reads the current login information.
  Example Usage
  
  data "docker_login" "current" {}
  
  output "current_user" {
  	value = data.docker_login.current.username
  }
---

# docker_login (Data Source)

Reads the current login information.

## Example Usage

```hcl
data "docker_login" "current" {}

output "current_user" {
	value = data.docker_login.current.username
}
```



<!-- schema generated by tfplugindocs -->
## Schema

### Read-Only

- `username` (String) Current username
