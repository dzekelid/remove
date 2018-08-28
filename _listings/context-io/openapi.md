swagger: "2.0"
x-collection-name: Context.IO
x-complete: 1
info:
  title: Context.IO
  description: context-io-is-the-missing-email-api-that-makes-it-easy-and-fast-to-integrate-your-users-email-data-in-your-application-
  version: 1.0.0
host: api.context.io
basePath: /2.0/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{id}:
    delete:
      summary: Delete Accounts
      description: Removes a given account.
      operationId: removeAccount_
      x-api-path-slug: accountsid-delete
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
  /accounts/{id}/connect_tokens/{token}:
    delete:
      summary: Delete Accounts Connect Tokens Token
      description: Remove a given connect token.
      operationId: removeAccountConnectToken_
      x-api-path-slug: accountsidconnect-tokenstoken-delete
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: token
        description: The unique random token used to add a second source to an existing
          account
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Connect
      - Tokens
      - Token
  /accounts/{id}/email_addresses/{email}:
    delete:
      summary: Delete Accounts Email Addresses Email
      description: Removes an email address form the aliases of an account.
      operationId: removeAccountEmailAddress_
      x-api-path-slug: accountsidemail-addressesemail-delete
      parameters:
      - in: path
        name: email
        description: One of the email addresses associated to the account
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Email
      - Addresses
      - Email
  /accounts/{id}/sources/{label}:
    delete:
      summary: Delete Accounts Sources Label
      description: Removes a data source of an account.
      operationId: removeAccountSource_
      x-api-path-slug: accountsidsourceslabel-delete
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: label
        description: The label property of the source instance
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Sources
      - Label