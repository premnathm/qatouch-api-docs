## QA Touch API

Before you start using our **API**, your first step is to obtain an `api-token` from your QA Touch site. Once you obtain the token, then you are ready to go.

## Requirements

All the API endpoints require a couple of headers so that we can authenticate you before processing the request.

**Required Headers**

1. domain
2. api-token

## Pagination

By default, all the endpoints which return more than 50 rows are paginated. You can move to another page by adding parameters to the request.

For example : `api.qatouch.com/api/v1/getAllProjects?page=2`

The above example will return the data which are available in the second page of the request.