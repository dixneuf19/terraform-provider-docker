---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "docker_hub_repository Resource - docker"
subcategory: ""
description: |-
  Manages an image repository in your account or organization.
  ~> Note When used with a Personal Access Token authentication (PAT), the PAT should
  have the "Read, Write, and Delete" scope to create and delete repositories. The
  owner of the PAT must be an editor of the org.
  Example Usage
  
  resource "docker_hub_repository" "example" {
  	namespace       = "my-organization"
  	name            = "my-repo"
  	description     = "A repository for storing container images"
  	full_description = "This repository stores container images for the development team."
  	private         = true
  }
---

# docker_hub_repository (Resource)

Manages an image repository in your account or organization.

~> **Note** When used with a Personal Access Token authentication (PAT), the PAT should
have the "Read, Write, and Delete" scope to create and delete repositories. The
owner of the PAT must be an editor of the org.

## Example Usage

```hcl
resource "docker_hub_repository" "example" {
	namespace       = "my-organization"
	name            = "my-repo"
	description     = "A repository for storing container images"
	full_description = "This repository stores container images for the development team."
	private         = true
}
```



<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `name` (String) Repository name
- `namespace` (String) Repository namespace

### Optional

- `description` (String) Repository description
- `full_description` (String) Repository full description
- `private` (Boolean) Is the repository private

### Read-Only

- `id` (String) The namespace/name of the repository
- `pull_count` (Number)
