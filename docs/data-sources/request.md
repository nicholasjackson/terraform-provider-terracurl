---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "terracurl_request Data Source - terraform-provider-terracurl"
subcategory: ""
description: |-
  Sample data source in the Terraform provider scaffolding.
---

# terracurl_request (Data Source)

Sample data source in the Terraform provider scaffolding.

## Example Usage
```hcl
data "terracurl_request" "test" {
  name           = "products"
  url            = "https://api.releases.hashicorp.com/v1/products"
  method         = "GET"
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `method` (String) HTTP method to use in the API call
- `name` (String) Friendly name for this API call
- `url` (String) Api endpoint to call

### Optional

- `headers` (Map of String) Map of headers to attach to the API call
- `request_body` (String) A request body to attach to the API call

### Read-Only

- `id` (String) The ID of this resource.
- `response` (String) JSON response received from request

