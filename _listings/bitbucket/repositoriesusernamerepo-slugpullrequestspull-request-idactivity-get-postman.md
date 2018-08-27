{
  "info": {
    "name": "Bitbucket Get Repositories Username Repo Slug Pullrequests Pull Request  Activity",
    "_postman_id": "e2ef048b-3cdc-4133-bfbd-59c052468e43",
    "description": "Returns a paginated list of the pull request's activity log.\n\nThis includes comments that were made by the reviewers, updates and\napprovals.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "repositories",
      "item": [
        {
          "id": "1da9f7da-802b-405c-984e-2f0a2c7d4618",
          "name": "getRepositoriesUsernameRepoSlugPullrequestsPullRequestActivity",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bitbucket.org",
              "path": [
                "2.0",
                "repositories/:username/:repo_slug/pullrequests/:pull_request_id/activity"
              ],
              "variable": [
                {
                  "id": "pull_request_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "repo_slug",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "username",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a paginated list of the pull request's activity log"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "185aeb3e-fcad-4583-b483-72c0e452e2ae"
            }
          ]
        }
      ]
    }
  ]
}