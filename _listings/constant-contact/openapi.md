swagger: "2.0"
x-collection-name: Constant Contact
x-complete: 1
info:
  title: ConstantContact
  description: constant-contact-inc-is-an-online-marketing-company-offering-email-marketing-social-media-marketing-online-survey-and-event-marketing-tools-primarily-to-small-businesses-nonprofit-organizations-and-membership-associations-
  termsOfService: http://www.constantcontact.com/uidocs/CCSiteOwnerAgreement.jsp
  version: 1.0.0
host: api.constantcontact.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{username}/activities:
    post:
      summary: Add Activity
      description: Add Activity
      operationId: add-activity
      x-api-path-slug: usernameactivities-post
      parameters:
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Activity
  /{username}/activities/{activity-id}:
    get:
      summary: Get Activity
      description: Get Activity
      operationId: get-activity
      x-api-path-slug: usernameactivitiesactivityid-get
      parameters:
      - in: path
        name: activity-id
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Activity