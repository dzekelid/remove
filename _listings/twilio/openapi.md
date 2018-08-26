---
swagger: "2.0"
x-collection-name: Twilio
x-complete: 1
info:
  title: Twilio
  description: twilio-is-a-cloud-communications-infrastructure-as-a-serviceiaas-company-based-in-san-francisco-california--twilio-allows-software-developers-to-programmatically-make-and-receive-phone-calls-and-send-and-receive-text-messages-using-its-web-service-apis--twilios-services-are-accessed-over-http-and-are-billed-based-on-usage-
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
  /Accounts/{AccountSid}/SIP/CredentialLists/{CLSid}/Credentials/{CredentialSid}:
    delete:
      summary: Delete SIP Credential From List
      description: Remove a Credential from a CredentialList.
      operationId: remove-a-credential-from-a-credentiallist
      x-api-path-slug: accountsaccountsidsipcredentiallistsclsidcredentialscredentialsid-delete
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: CLSid
        description: A 34 character string that uniquely identifies the credential
          list
      - in: path
        name: CredentialSid
      responses:
        200:
          description: OK
      tags:
      - SIP Credential Lists
  /Accounts/{AccountSid}/SIP/Domains/{SipDomainSid}/CredentialListMappings/{CLSid}:
    delete:
      summary: Delete Domains Credentials
      description: Remove a CredentialListMapping from a domain
      operationId: remove-a-credentiallistmapping-from-a-domain
      x-api-path-slug: accountsaccountsidsipdomainssipdomainsidcredentiallistmappingsclsid-delete
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: CLSid
        description: A 34 character string that uniquely identifies the credential
          list
      - in: path
        name: SipDomainSid
        description: A 34 character string that uniquely identifies the SIP domain
      responses:
        200:
          description: OK
      tags:
      - SIP Domains
  /Accounts/{AccountSid}/SIP/Domains/{SipDomainSid}/IpAccessControlListMappings/{ALSid}:
    delete:
      summary: Delete Domains Credentials
      description: Remove a mapping from this domain.
      operationId: remove-a-mapping-from-this-domain
      x-api-path-slug: accountsaccountsidsipdomainssipdomainsidipaccesscontrollistmappingsalsid-delete
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: ALSid
      - in: path
        name: SipDomainSid
        description: A 34 character string that uniquely identifies the SIP domain
      responses:
        200:
          description: OK
      tags:
      - SIP Domains
---