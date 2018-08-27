{
  "info": {
    "name": "Bitbucket Get Repositories Username Repo Slug Pullrequests Activity",
    "_postman_id": "560bd493-9e7a-48a8-b1f6-a1d690db4967",
    "description": "Returns a paginated list of the pull request's activity log.\n\nThis includes comments that were made by the reviewers, updates and\napprovals.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "repositories",
      "item": [
        {
          "id": "a6e0ce72-f969-47a9-b12f-bc60ed7fe9cd",
          "name": "getRepositoriesUsernameRepoSlugPullrequestsActivity",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bitbucket.org",
              "path": [
                "2.0",
                "repositories/:username/:repo_slug/pullrequests/activity"
              ],
              "variable": [
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
              "id": "ee8d5467-bb4d-46f8-8ec0-0029096754ac"
            }
          ]
        }
      ]
    }
  ]
}