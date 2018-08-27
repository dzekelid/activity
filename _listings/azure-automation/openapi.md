swagger: "2.0"
x-collection-name: Azure Automation
x-complete: 1
info:
  title: AutomationManagementClient
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts/{automationAccountName}/modules/{moduleName}/activities/{activityName}
  : get:
      summary: Activity Get
      description: Retrieve the activity in the module identified by module name and
        activity name.
      operationId: Activity_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamemodulesmodulenameactivitiesactivityname-get
      parameters:
      - in: path
        name: activityName
        description: The name of activity
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: path
        name: moduleName
        description: The name of module
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Activity
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts/{automationAccountName}/modules/{moduleName}/activities
  : get:
      summary: Activity List By Module
      description: Retrieve a list of activities in the module identified by module
        name.
      operationId: Activity_ListByModule
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamemodulesmodulenameactivities-get
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: path
        name: moduleName
        description: The name of module
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Activity
      - ListModule