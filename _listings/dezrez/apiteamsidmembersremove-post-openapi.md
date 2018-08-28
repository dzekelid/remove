---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Remove a member from a team
  version: 1.0.0
  description: Remove a member from a team.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/accounting/exports/batch/{id}/removepayment:
    put:
      summary: Remove an individual payment from batch export
      description: Remove an individual payment from batch export.
      operationId: AccountingExport_RemoveFromBatchByidBypaymentId
      x-api-path-slug: apiaccountingexportsbatchidremovepayment-put
      parameters:
      - in: path
        name: id
      - in: query
        name: paymentId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Individual
      - Payment
      - From
      - Batch
      - Export
  /api/auction/removecontact:
    post:
      summary: Remove an existing auction contact from the auction role
      description: Remove an existing auction contact from the auction role.
      operationId: Auction_RemoveAuctionContactByremoveContactDataContract
      x-api-path-slug: apiauctionremovecontact-post
      parameters:
      - in: body
        name: removeContactDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Existing
      - Auction
      - Contact
      - From
      - Auction
      - Role
  /api/dashboard/{id}/removewidgets:
    put:
      summary: Remove widgets from a dashboard
      description: Remove widgets from a dashboard.
      operationId: Dashboard_RemoveWidgetsFromDashboardByid
      x-api-path-slug: apidashboardidremovewidgets-put
      parameters:
      - in: path
        name: id
        description: Dashboard Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Widgets
      - From
      - Dashboard
  /api/group/{id}/removepreferredcompany:
    post:
      summary: Remove a preferred company to a group
      description: Remove a preferred company to a group.
      operationId: Group_RemovePreferredCompanyByidBycompanyId
      x-api-path-slug: apigroupidremovepreferredcompany-post
      parameters:
      - in: query
        name: companyId
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Preferred
      - Company
      - To
      - Group
  /api/invoice/{id}/removefee:
    put:
      summary: Remove fee from existing invoice
      description: Remove fee from existing invoice.
      operationId: Invoice_RemoveLinkedFeeByidByattachedFeeId
      x-api-path-slug: apiinvoiceidremovefee-put
      parameters:
      - in: query
        name: attachedFeeId
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Fee
      - From
      - Existing
      - Invoice
  /api/invoice/removereceiptallocation:
    delete:
      summary: Remove a receipt list item allocation
      description: Remove a receipt list item allocation.
      operationId: Invoice_RemoveSavedReceiptItemAllocationByreceiptItemIdByinvoiceIdByallocationId
      x-api-path-slug: apiinvoiceremovereceiptallocation-delete
      parameters:
      - in: query
        name: allocationId
      - in: query
        name: invoiceId
      - in: query
        name: receiptItemId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Receipt
      - List
      - Item
      - Ocation
  /api/role/lettings/{roleId}/removeutility:
    delete:
      summary: Remove a utility for the letting role
      description: Remove a utility for the letting role.
      operationId: LettingRole_RemoveUtilityUtilityByroleIdByutilityId
      x-api-path-slug: apirolelettingsroleidremoveutility-delete
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: roleId
        description: The letting role Id
      - in: query
        name: utilityId
        description: The utility Id
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Utilitythe
      - Letting
      - Role
  /api/role/lettings/{id}/removeadditionalservice/{additionalServiceId}:
    post:
      summary: Remove additional service to lettings role tenancy
      description: Remove additional service to lettings role tenancy.
      operationId: LettingRole_DeleteAdditionalServiceByidByadditionalServiceId
      x-api-path-slug: apirolelettingsidremoveadditionalserviceadditionalserviceid-post
      parameters:
      - in: path
        name: additionalServiceId
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Additional
      - Service
      - To
      - Lettings
      - Role
      - Tenancy
  /api/progression/lettings/{roleId}/removetenantcharge:
    delete:
      summary: Remove charges from a tenant role
      description: Remove charges from a tenant role.
      operationId: LettingsProgression_RemoveTenantChargesByroleIdBychargeIds
      x-api-path-slug: apiprogressionlettingsroleidremovetenantcharge-delete
      parameters:
      - in: query
        name: chargeIds
        description: The ids of the charges to remove
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: roleId
        description: The tenant role id
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Charges
      - From
      - Tenant
      - Role
  /api/negotiator/my/properties/favourite/remove/{propertyId}:
    delete:
      summary: Remove a property from a Negotiators favourite list.
      description: Remove a property from a negotiators favourite list..
      operationId: Negotiator_RemoveFavouritePropertyBypropertyIdByroleId
      x-api-path-slug: apinegotiatormypropertiesfavouriteremovepropertyid-delete
      parameters:
      - in: path
        name: propertyId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: roleId
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Property
      - From
      - Negotiators
      - Favourite
      - List
  /api/negotiator/my/groups/favourite/remove/{groupId}:
    delete:
      summary: Remove a group from a Negotiators favourite list.
      description: Remove a group from a negotiators favourite list..
      operationId: Negotiator_RemoveFavouriteGroupBygroupId
      x-api-path-slug: apinegotiatormygroupsfavouriteremovegroupid-delete
      parameters:
      - in: path
        name: groupId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Group
      - From
      - Negotiators
      - Favourite
      - List
  /api/people/{id}/removecontactitem/{contactItemid}:
    put:
      summary: Remove a ContactItem from a Person
      description: Remove a contactitem from a person.
      operationId: People_RemoveContactItemByidBycontactItemid
      x-api-path-slug: apipeopleidremovecontactitemcontactitemid-put
      parameters:
      - in: path
        name: contactItemid
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - ContactItem
      - From
      - Person
  /api/people/{id}/removeaddress/{addressId}:
    put:
      summary: Remove an Address from a Person
      description: Remove an address from a person.
      operationId: People_RemoveAddressByidByaddressId
      x-api-path-slug: apipeopleidremoveaddressaddressid-put
      parameters:
      - in: path
        name: addressId
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Ress
      - From
      - Person
  /api/progression/removecontact:
    post:
      summary: Remove an existing progression contact from the progression role
      description: Remove an existing progression contact from the progression role.
      operationId: Progression_RemoveProgressionContactByremoveContactDataContract
      x-api-path-slug: apiprogressionremovecontact-post
      parameters:
      - in: body
        name: removeContactDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Existing
      - Progression
      - Contact
      - From
      - Progression
      - Role
  /api/progression/milestones/remove:
    put:
      summary: Remove a new milestone
      description: Remove a new milestone.
      operationId: Progression_RemoveMilestoneBypurchasingRoleIdBymilestoneId
      x-api-path-slug: apiprogressionmilestonesremove-put
      parameters:
      - in: query
        name: milestoneId
        description: Id of milestone to remove
      - in: query
        name: purchasingRoleId
        description: The purchasing role ID
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - New
      - Milestone
  /api/property/{id}/keys/remove:
    delete:
      summary: Remove keys from a property
      description: Remove keys from a property.
      operationId: Property_RemoveKeysByidBykeyIds
      x-api-path-slug: apipropertyidkeysremove-delete
      parameters:
      - in: path
        name: id
        description: The property id
      - in: query
        name: keyIds
        description: The ids of the keys to remove
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Keys
      - From
      - Property
  /api/property/{id}/alarms/remove:
    delete:
      summary: Remove alarm codes from a property
      description: Remove alarm codes from a property.
      operationId: Property_RemoveAlarmsByidByalarmIds
      x-api-path-slug: apipropertyidalarmsremove-delete
      parameters:
      - in: query
        name: alarmIds
        description: The ids of the alarm codes to remove
      - in: path
        name: id
        description: The property id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Alarm
      - Codes
      - From
      - Property
  /api/property/{id}/specialarrangements/remove:
    delete:
      summary: Remove special arrangements from a property
      description: Remove special arrangements from a property.
      operationId: Property_RemoveSpecialArrangementsByidByarrangementIds
      x-api-path-slug: apipropertyidspecialarrangementsremove-delete
      parameters:
      - in: query
        name: arrangementIds
        description: The ids of the special arrangements to remove
      - in: path
        name: id
        description: The property id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Special
      - Arrangements
      - From
      - Property
  /api/property/{id}/certificate/remove:
    delete:
      summary: Remove certificate from a property
      description: Remove certificate from a property.
      operationId: Property_RemoveCertificateByidBycertificateId
      x-api-path-slug: apipropertyidcertificateremove-delete
      parameters:
      - in: query
        name: certificateId
        description: The ids of the certificate to remove
      - in: path
        name: id
        description: The property id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Certificate
      - From
      - Property
  /api/region/favourites/{favouriteRegionId}:
    delete:
      summary: Remove a region from your favourites
      description: Remove a region from your favourites.
      operationId: Region_RemoveFavouriteByfavouriteRegionId
      x-api-path-slug: apiregionfavouritesfavouriteregionid-delete
      parameters:
      - in: path
        name: favouriteRegionId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Region
      - From
      - Your
      - Favourites
  /api/role/{id}/removefee:
    put:
      summary: Remove a fee from a given PropertyMarketingRole.
      description: Remove a fee from a given propertymarketingrole..
      operationId: Role_RemoveFeeByidByfeeId
      x-api-path-slug: apiroleidremovefee-put
      parameters:
      - in: query
        name: feeId
        description: The Id of the fee to remove
      - in: path
        name: id
        description: the id of the role
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Fee
      - From
      - Given
      - PropertyMarketingRole
  /api/role/{id}/removeholdingdeposit:
    post:
      summary: Remove holding deposit from role
      description: Remove holding deposit from role.
      operationId: Role_RemoveHoldingDepositByidByrelatedRoleId
      x-api-path-slug: apiroleidremoveholdingdeposit-post
      parameters:
      - in: path
        name: id
      - in: query
        name: relatedRoleId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Holding
      - Deposit
      - From
      - Role
  /api/teams/{id}/members/remove:
    post:
      summary: Remove a member from a team
      description: Remove a member from a team.
      operationId: Teams_RemoveMemberByidByremoveTeamMemberCommand
      x-api-path-slug: apiteamsidmembersremove-post
      parameters:
      - in: path
        name: id
        description: Team Id
      - in: body
        name: removeTeamMemberCommand
        description: Details of team members
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Member
      - From
      - Team
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