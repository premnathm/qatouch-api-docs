## Projects

### List Projects

Provides the list of projects created for your domain.

```
POST api.qatouch.com/api/v1/getAllProjects
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

### Create Project

Create a new project in your domain.

```
POST api.qatouch.com/api/v1/project
```
#### Example request

```curl
curl --location --request POST "api.qatouch.com/api/v1/project?name=Automation" \
  --header "api-token: " \
  --header "domain: " \
  --data ""
```

| Headers       | Description                |
| ------------- | ------------- |
| domain  | Your QA Touch domain.  |
| api-token  | Your secret api-token.  |

| Parameters  | Description|
| ------------- | ------------- |
| name  | Name of the new Project to be created  |

## Test Cases

### List Test Cases

Provides the list of test cases available for the project.

```
GET api.qatouch.com/api/v1/getAllTestCases/{projectKey}
```
#### Example request

```curl
curl --location --request GET "api.qatouch.com/api/v1/getAllTestCases/{projectKey}" \
  --header "domain: {your-domain}" \
  --header "api-token: {your-api-token}" \
  --data ""
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

### List all Modules

Provides the list of Modules available for the project.

```
GET api.qatouch.com/api/v1/getAllModules/{projectKey}
```
#### Example request

```curl
curl --location --request POST "api.qatouch.com/api/v1/getAllModules/{projectKey}" \
  --header "api-token: {your-api-token}" \
  --header "domain: {your-domain}" \
  --data ""
```

| Headers       | Description|
| ------------- | ------------- |
| domain  | Your QA Touch domain.  |
| api-token  | Your secret api-token.  |


### Create Module

Create a new module in your project for Test Case.

```
POST api.qatouch.com/api/v1/module
```
#### Example request

```curl
curl --location --request POST "api.qatouch.com/api/v1/module?projectKey={projectKey}&moduleName={moduleName}" \
  --header "api-token: {your-api-token}" \
  --header "domain: {your-domain}" \
  --data ""
```

| Headers       | Description|
| ------------- | ------------- |
| domain  | Your QA Touch domain.  |
| api-token  | Your secret api-token.  |


| Parameters  | Description|
| ------------- | ------------- |
| projectKey  | Project Key under which the Module to be created  |
| moduleName  | Name of the module to be created  |
| parentKey  | (Optional) To create child module, provide this parameter with existing Module's Key  |

### Create Test Cases

Create a new Test Cases in your project.

```
POST api.qatouch.com/api/v1/testCase?projectKey={projectKey}&sectionKey={sectionKey}&caseTitle={caseTitle}
```
#### Example request

```curl
curl --location --request POST "api.qatouch.com/api/v1/module?projectKey={projectKey}&moduleName={moduleName}" \
  --header "api-token: {your-api-token}" \
  --header "domain: {your-domain}" \
  --data ""
```

| Headers       | Description|
| ------------- | ------------- |
| domain  | Your QA Touch domain.  |
| api-token  | Your secret api-token.  |


| Parameters  | Description|
| ------------- | ------------- |
| projectKey  | Project Key under which the Module to be created  |
| sectionKey  | Provide the section key for under which the test case should be created  |
| caseTitle  | Title of the test case   |

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

### Create Milestone

Create a new Milestone in your project.

```
POST api.qatouch.com/api/v1/milestone
```
#### Example request

```curl
curl --location --request POST "api.qatouch.com/api/v1/milestone?projectKey={projectKey}&milestone={milestone} \
  --header "api-token: {your-api-token}" \
  --header "domain: {your-domain}" \
  --data ""
```

| Headers       | Description|
| ------------- | ------------- |
| domain  | Your QA Touch domain.  |
| api-token  | Your secret api-token.  |


| Parameters  | Description|
| ------------- | ------------- |
| projectKey  | Project Key under which the Milestone to be created  |
| milestone  | Name of the milestone to be created  |

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

### List all available Users for Testing

Provides the list of Users in the project available for Testing.

```
GET api.qatouch.com/api/v1/testRun/availableUsers/{projectKey}
```

#### Example request

```curl
curl --location --request GET "api.qatouch.com/api/v1/testRun/availableUsers/{projectKey}" \
  --header "domain: {your-domain}" \
  --header "api-token: {your-api-token}" \
  --data ""
```

| Headers       | Description|
| ------------- | ------------- |
| domain  | Your QA Touch domain.  |
| api-token  | Your secret api-token.  |

### Create Test Run

Create a new Test Run in your project.

```
POST api.qatouch.com/api/v1/testRun
```
#### Example request

```curl
curl --location --request POST "api.qatouch.com/api/v1/testRun?projectKey={projectKey}&assignTo={assignTo}&milestoneKey={milestoneKey}&testRun={testRun} \
  --header "api-token: {your-api-token}" \
  --header "domain: {your-domain}" \
  --data ""
```

| Headers       | Description|
| ------------- | ------------- |
| domain  | Your QA Touch domain.  |
| api-token  | Your secret api-token.  |


| Parameters  | Description|
| ------------- | ------------- |
| projectKey  | Project Key under which the Test Run to be created  |
| assignTo  | User key to which the Test Run to be assigned  |
| milestoneKey  | Provide the milestone key to be assigned to Test Run  |
| testRun  | Title of the Test Run  |


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


### Create Defect

Create a new Defect in your project.

```
POST api.qatouch.com/api/v1/defects
```
#### Example request

```curl
curl --location --request POST "api.qatouch.com/api/v1/defects?projectKey={projectKey}&priority={priority}&issueSummary={issueSummary} \
  --header "api-token: {your-api-token}" \
  --header "domain: {your-domain}" \
  --data ""
```

| Headers       | Description|
| ------------- | ------------- |
| domain  | Your QA Touch domain.  |
| api-token  | Your secret api-token.  |


| Parameters  | Description|
| ------------- | ------------- |
| projectKey  | Project Key under which the Defect to be created  |
| priority  | Priority to be given to the Defect |
| issueSummary  | Title of the Defect  |

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
