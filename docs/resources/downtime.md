---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "downtime Resource - obmprovider"
subcategory: ""
description: |-
  
---

# downtime (Resource)





<!-- schema generated by tfplugindocs -->
## Schema

### Required

- **action** (String) A value which represents the downtime action name
- **approver** (String) Name of the approver of the downtime
- **category** (String) A value which represents the downtime category name
- **description** (String)
- **name** (String) Name of the downtime
- **schedule** (Block Set, Min: 1, Max: 1) (see [below for nested schema](#nestedblock--schedule))
- **selected_cis** (Set of String) List of configuration items impacted by the downtime

### Optional

- **id** (String) The ID of this resource.
- **last_updated** (String)

<a id="nestedblock--schedule"></a>
### Nested Schema for `schedule`

Required:

- **end_date** (String) The downtime end date specified as the RFC 3339 date-time format: yyyy-MM-dd'T'HH:mm:ss('+'/'-')HH:mm
- **start_date** (String) The downtime start date specified as the RFC 3339 date-time format: yyyy-MM-dd'T'HH:mm:ss('+'/'-')HH:mm
- **timezone** (String) Timezone
- **type** (String) Must be set to ONCE. The donwtime occurs only once on a specified start date and lasts till a specified end date

