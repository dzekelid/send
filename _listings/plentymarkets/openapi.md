swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 1
info:
  title: plentymarkets REST-API
  description: the-plentymarkets-rest-api-expands-the-functionality-of-the-plentymarkets-cms-and-allows-access-to-resources-i-e--data-records-via-unique-uri-paths
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/accounts/contacts/{contactId}/access_data/new_password:
    put:
      summary: Send password link for a contact
      description: Sends an email to a contact with a link to change the password.
        The ID of the contact must be specified.
      operationId: putRestAccountsContactsContactAccessDataNewPassword
      x-api-path-slug: restaccountscontactscontactidaccess-datanew-password-put
      parameters:
      - in: path
        name: contactId
      - in: query
        name: password
        description: The new password
      responses:
        200:
          description: OK
      tags:
      - Send
      - Password
      - Linka
      - Contact
  /rest/plugins_mail:
    post:
      summary: Send mail
      description: Send mail from booted plugins.
      operationId: postRestPluginsMail
      x-api-path-slug: restplugins-mail-post
      responses:
        200:
          description: OK
      tags:
      - Send
      - Mail