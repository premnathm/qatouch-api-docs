## Projects

### List Projects

Provides the list of projects created for your domain.

```
GET api.qatouch.com/api/v1/getAllProjects
```
#### Example request

```curl
curl --location --request GET "api.qatouch.com/api/v1/getAllProjects" \
  --header "domain: {your-domain}" \
  --header "api-token: {your-api-token}" \
  --data ""
```

| Headers       | Description                |
| ------------- | ------------- |
| domain  | Your QA Touch domain.  |
| api-token  | Your secret api-token.  |


### Count Projects

Count of the total projects available.

```
GET api.qatouch.com/api/v1/count/allProjects
```
#### Example request

```curl
curl --location --request GET "api.qatouch.com/api/v1/count/allProjects" \
  --header "domain: {your-domain}" \
  --header "api-token: {your-api-token}" \
  --data ""
```

| Headers       | Description                |
| ------------- | ------------- |
| domain  | Your QA Touch domain.  |
| api-token  | Your secret api-token.  |

## Test Cases

### List Test Cases

Provides the list of test cases available for the project.

```
GET api.qatouch.com/api/v1/getAllTestCases/{projectKey}
```

| Headers       | Description                |
| ------------- | ------------- |
| domain  | Your QA Touch domain.  |
| api-token  | Your secret api-token.  |

### Count Test Cases

Count of the total test cases available for the project.

```
GET api.qatouch.com/api/v1/count/allTestCases/{projectKey}
```
#### Example request

```curl
curl --location --request GET "api.qatouch.com/api/v1/count/allTestCases/{projectKey}" \
  --header "domain: {your-domain}" \
  --header "api-token: {your-api-token}" \
  --data ""
```

| Headers       | Description|
| ------------- | ------------- |
| domain  | Your QA Touch domain.  |
| api-token  | Your secret api-token.  |

## Milestones

### List Milestones

Provides the list of Milestones available for the project.

```
GET api.qatouch.com/api/v1/getAllMilestones/{projectKey}
```
#### Example request

```curl
curl --location --request GET "api.qatouch.com/api/v1/getAllMilestones/{projectKey}" \
  --header "domain: {your-domain}" \
  --header "api-token: {your-api-token}" \
  --data ""
```

| Headers       | Description |
| ------------- | ------------- |
| domain  | Your QA Touch domain.  |
| api-token  | Your secret api-token.  |

### Count Milestones

Count of the total Milestones available for the project.

```
GET api.qatouch.com/api/v1/count/allMilestones/{projectKey}
```
#### Example request

```curl
curl --location --request GET "api.qatouch.com/api/v1/count/allMilestones/{projectKey}" \
  --header "domain: {your-domain}" \
  --header "api-token: {your-api-token}" \
  --data ""
```

| Headers       | Description|
| ------------- | ------------- |
| domain  | Your QA Touch domain.  |
| api-token  | Your secret api-token.  |

## Test Runs

### List Test Runs

Provides the list of Test Runs available for the project.

```
GET api.qatouch.com/api/v1/getAllTestRuns/{projectKey}
```

#### Example request

```curl
curl --location --request GET "api.qatouch.com/api/v1/getAllTestRuns/{projectKey}" \
  --header "domain: {your-domain}" \
  --header "api-token: {your-api-token}" \
  --data ""
```

| Headers       | Description|
| ------------- | ------------- |
| domain  | Your QA Touch domain.  |
| api-token  | Your secret api-token.  |

### Count Test Runs

Count of the total Test Runs available for the project.

```
GET api.qatouch.com/api/v1/count/allTestRuns/{projectKey}
```
#### Example request

```curl
curl --location --request GET "api.qatouch.com/api/v1/count/allTestRuns/{projectKey}" \
  --header "domain: {your-domain}" \
  --header "api-token: {your-api-token}" \
  --data ""
```

| Headers       | Description|
| ------------- | ------------- |
| domain  | Your QA Touch domain.  |
| api-token  | Your secret api-token.  |

### List Test Run Results

Provides the list of Test Runs Results available for a Test Run.

```
GET api.qatouch.com/api/v1/testRunResults/{projectKey}/{testRunKey}
```
#### Example request

```curl
curl --location --request GET "api.qatouch.com/api/v1/testRunResults/{projectKey}/{testRunKey}" \
  --header "domain: {your-domain}" \
  --header "api-token: {your-api-token}" \
  --data ""
```

| Headers       | Description|
| ------------- | ------------- |
| domain  | Your QA Touch domain.  |
| api-token  | Your secret api-token.  |

### List Test Run Results History

Provides the list of History(s) available of Test Runs Results.

```
GET api.qatouch.com/api/v1/testRunResults/history/{projectKey}/{testRunKey}/{resultKey}
```
#### Example request

```curl
curl --location --request GET "api.qatouch.com/api/v1/testRunResults/history/{projectKey}/{testRunKey}/{resultKey}" \
  --header "domain: {your-domain}" \
  --header "api-token: {your-api-token}" \
  --data ""
```

| Headers       | Description|
| ------------- | ------------- |
| domain  | Your QA Touch domain.  |
| api-token  | Your secret api-token.  |


### List Statuses for Test Run

Provides the list of available statuses for Test Runs.

```
GET api.qatouch.com/api/v1/testRuns/getAvailableStatuses
```
#### Example request

```curl
curl --location --request GET "api.qatouch.com/api/v1/testRuns/getAvailableStatuses" \
  --header "domain: {your-domain}" \
  --header "api-token: {your-api-token}" \
  --data ""
```

| Headers       | Description|
| ------------- | ------------- |
| domain  | Your QA Touch domain.  |
| api-token  | Your secret api-token.  |


### Update Test Run Status

Update the status for the test run.

```
PATCH api.qatouch.com/api/v1/testRunResults/status?status={status}&project={projectKey}&test_run={testRunKey}&run_result={resultKey}
```

#### Example request

```curl
curl --location --request PATCH "api.qatouchapi.com/api/v1/testRunResults/status?status={status}&project={projectKey}&test_run={testRunKey}&run_result={runResultKey}" \
  --header "api-token: {your-api-token}" \
  --header "domain: {your-domain}" \
  --data ""
```

| Headers    | Description|
| ------------- | ------------- |
| domain  | Your QA Touch domain.  |
| api-token  | Your secret api-token.  |

| Parameters  | Description|
| ------------- | ------------- |
| status  | Status to be updated.  |
| project  | Project Key.  |
| test_run  | Test Run Key.  |
| run_result  | Test Run Result Key.  


## Defects

### List Defects

Provides the list of Defects available for the project.

```
GET api.qatouch.com/api/v1/getAllDefects/{projectKey}
```
#### Example request

```curl
curl --location --request GET "api.qatouch.com/api/v1/getAllDefects/{projectKey}" \
  --header "domain: {your-domain}" \
  --header "api-token: {your-api-token}" \
  --data ""
```

| Headers    | Description|
| ------------- | ------------- |
| domain  | Your QA Touch domain.  |
| api-token  | Your secret api-token.  |

### List Defects Statuses

Provides the list of available defect statuses.

```
GET api.qatouch.com/api/v1/defects/status
```
#### Example request

```curl
curl --location --request GET "api.qatouch.com/api/v1/defects/status" \
  --header "domain: {your-domain}" \
  --header "api-token: {your-api-token}" \
  --data ""
```

| Headers    | Description|
| ------------- | ------------- |
| domain  | Your QA Touch domain.  |
| api-token  | Your secret api-token.  |

### List Defects Severity

Provides the list of available defect severity.

```
GET api.qatouch.com/api/v1/defects/severity
```
#### Example request

```curl
curl --location --request GET "api.qatouch.com/api/v1/defects/severity" \
  --header "domain: {your-domain}" \
  --header "api-token: {your-api-token}" \
  --data ""
```

| Headers    | Description|
| ------------- | ------------- |
| domain  | Your QA Touch domain.  |
| api-token  | Your secret api-token.  

### List Defects Issue Type

Provides the list of available defect Issue Type.

```
GET api.qatouch.com/api/v1/defects/issueType
```
#### Example request

```curl
curl --location --request GET "api.qatouch.com/api/v1/defects/issueType" \
  --header "domain: {your-domain}" \
  --header "api-token: {your-api-token}" \
  --data ""
```

| Headers    | Description|
| ------------- | ------------- |
| domain  | Your QA Touch domain.  |
| api-token  | Your secret api-token.  |

### List Defects Environments

Provides the list of available defect environments.

```
GET api.qatouch.com/api/v1/defects/environment
```
#### Example request

```curl
curl --location --request GET "api.qatouch.com/api/v1/defects/environment" \
  --header "domain: {your-domain}" \
  --header "api-token: {your-api-token}" \
  --data ""
```

| Headers    | Description|
| ------------- | ------------- |
| domain  | Your QA Touch domain.  |
| api-token  | Your secret api-token.  |

### Count Defects

Count of the total Defects available for the project.

```
GET api.qatouch.com/api/v1/count/allDefects/{projectKey}
```
#### Example request

```curl
curl --location --request GET "api.qatouch.com/api/v1/count/allDefects/{projectKey}" \
  --header "domain: {your-domain}" \
  --header "api-token: {your-api-token}" \
  --data ""
```

| Headers       | Description|
| ------------- | ------------- |
| domain  | Your QA Touch domain.  |
| api-token  | Your secret api-token.  |


## Requirements

### List Requirements

Provides the list of Requirements available for the project.

```
GET api.qatouch.com/api/v1/getAllRequirements/{projectKey}
```
#### Example request

```curl
curl --location --request GET "api.qatouch.com/api/v1/getAllRequirements/{projectKey}" \
  --header "domain: {your-domain}" \
  --header "api-token: {your-api-token}" \
  --data ""
```

| Headers       | Description|
| ------------- | ------------- |
| domain  | Your QA Touch domain.  |
| api-token  | Your secret api-token.  |

### Count Requirements

Count of the total Requirements available for the project.

```
GET api.qatouch.com/api/v1/count/allRequirements/{projectKey}
```
#### Example request

```curl
curl --location --request GET "api.qatouch.com/api/v1/count/allRequirements/{projectKey}" \
  --header "domain: {your-domain}" \
  --header "api-token: {your-api-token}" \
  --data ""
```

| Headers       | Description|
| ------------- | ------------- |
| domain  | Your QA Touch domain.  |
| api-token  | Your secret api-token.  |
