---
swagger: "2.0"
x-collection-name: Twilio
x-complete: 0
info:
  title: Twilio Get Incoming Local Phone Numbers
  description: Returns a list of local <IncomingPhoneNumber> elements, each representing
    a local (not toll-free) phone number given to your account, under an <IncomingPhoneNumbers>
    list element that includes paging information. Works exactly the same as the IncomingPhoneNumber
    resource, but filters out toll-free numbers.
  termsOfService: https://www.twilio.com/legal/tos
  version: v1
host: api.twilio.com
basePath: /2010-04-01/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Accounts/{AccountSid}/IncomingPhoneNumbers/Local.{format}:
    get:
      summary: Get Incoming Local Phone Numbers
      description: Returns a list of local <IncomingPhoneNumber> elements, each representing
        a local (not toll-free) phone number given to your account, under an <IncomingPhoneNumbers>
        list element that includes paging information. Works exactly the same as the
        IncomingPhoneNumber resource, but filters out toll-free numbers.
      operationId: returns-a-list-of-local-incomingphonenumber-elements-each-representing-a-local-not-tollfree-phone-nu
      x-api-path-slug: accountsaccountsidincomingphonenumberslocal-format-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: format
        description: By default, Twilios REST API returns XML
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Incoming Phone Numbers
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---