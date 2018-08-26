---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/documentgeneration/confirmationofviewing:
    post:
      summary: Generates a correspondence to notify all parties of a scheduled viewing.  Uses
        default values where possible.
      description: Generates a correspondence to notify all parties of a scheduled
        viewing.  uses default values where possible..
      operationId: DocumentGeneration_ConfirmationOfViewingPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationconfirmationofviewing-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Notify
      - ""
      - Parties
      - Of
      - Scheduled
      - Viewing
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/cancellationofviewing:
    post:
      summary: Generates a correspondence to notify parties of a cancellation of a
        viewing.  Uses default values where possible.
      description: Generates a correspondence to notify parties of a cancellation
        of a viewing.  uses default values where possible..
      operationId: DocumentGeneration_CancellationOfViewingPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationcancellationofviewing-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Notify
      - Parties
      - Of
      - Cancellation
      - Of
      - Viewing
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/reschedulingofviewing:
    post:
      summary: Generates a correspondence to notify parties involved of a rescheduling
        of a viewing.  Uses default values where possible.
      description: Generates a correspondence to notify parties involved of a rescheduling
        of a viewing.  uses default values where possible..
      operationId: DocumentGeneration_ReschedulingOfViewingPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationreschedulingofviewing-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Notify
      - Parties
      - Involved
      - Of
      - Rescheduling
      - Of
      - Viewing
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/viewing/feedback:
    post:
      summary: Sends viewing feedback to Owner / Landlord
      description: Sends viewing feedback to owner / landlord.
      operationId: DocumentGeneration_ViewingFeedbackBygeneratePackDataContract
      x-api-path-slug: apidocumentgenerationviewingfeedback-post
      parameters:
      - in: body
        name: generatePackDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Sends
      - Viewing
      - Feedback
      - To
      - Owner
      - ""
      - ""
      - Landlord
  /api/group/mostactive:
    get:
      summary: Return the Groups with the most viewings between a given date range,
        ordered by viewing Count
      description: Return the groups with the most viewings between a given date range,
        ordered by viewing count.
      operationId: Group_MostActiveBypageSizeByfilter.rangeFromByfilter.rangeToByfilter.branchIdByfilter.roleTypes
      x-api-path-slug: apigroupmostactive-get
      parameters:
      - in: query
        name: filter.branchId
      - in: query
        name: filter.rangeFrom
      - in: query
        name: filter.rangeTo
      - in: query
        name: filter.roleTypes
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Return
      - Groups
      - Most
      - Viewings
      - Between
      - Given
      - Date
      - Range
      - ""
      - Ordered
      - By
      - Viewing
      - Count
  /api/viewing/bookviewing:
    post:
      summary: Book a Viewing.
      description: Book a viewing..
      operationId: Viewing_BookViewingBybookViewingDataContract
      x-api-path-slug: apiviewingbookviewing-post
      parameters:
      - in: body
        name: bookViewingDataContract
        description: the viewing detail
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Book
      - Viewing
  /api/viewing/{id}/recordfeedback:
    post:
      summary: Record the feedback against a Viewing.
      description: Record the feedback against a viewing..
      operationId: Viewing_RecordFeedbackByidBycommand
      x-api-path-slug: apiviewingidrecordfeedback-post
      parameters:
      - in: body
        name: command
        description: Feedback details
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Viewing id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Record
      - Feedback
      - Against
      - Viewing
  /api/viewing/{id}/editfeedback:
    put:
      summary: Edit the feedback against a Viewing.
      description: Edit the feedback against a viewing..
      operationId: Viewing_EditFeedbackByidBycommand
      x-api-path-slug: apiviewingideditfeedback-put
      parameters:
      - in: body
        name: command
        description: Feedback details
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Viewing id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Edit
      - Feedback
      - Against
      - Viewing
  /api/viewing/{viewingFeedbackId}/feedbacknotified:
    post:
      summary: Record that the feedback for a Viewing was notified to the vendor.
      description: Record that the feedback for a viewing was notified to the vendor..
      operationId: Viewing_FeedbackNotifiedByviewingFeedbackIdBytypeBynotifiedDateBynegIds
      x-api-path-slug: apiviewingviewingfeedbackidfeedbacknotified-post
      parameters:
      - in: query
        name: negIds
      - in: query
        name: notifiedDate
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: type
        description: Task type for how vendor was communicated e
      - in: path
        name: viewingFeedbackId
        description: viewing feedback id
      responses:
        200:
          description: OK
      tags:
      - Record
      - That
      - Feedbacka
      - Viewing
      - Was
      - Notified
      - To
      - Vendor
  /api/viewing/{viewingFeedbackId}/editfeedbacknotified:
    put:
      summary: Edit that the feedback for a Viewing was notified to the vendor.
      description: Edit that the feedback for a viewing was notified to the vendor..
      operationId: Viewing_EditFeedbackNotifiedByviewingFeedbackIdByvendorNotifiedIdBytypeBynotifiedDateBynegIds
      x-api-path-slug: apiviewingviewingfeedbackideditfeedbacknotified-put
      parameters:
      - in: query
        name: negIds
      - in: query
        name: notifiedDate
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: type
        description: Task type for how vendor was communicated e
      - in: query
        name: vendorNotifiedId
        description: vendor notified id
      - in: path
        name: viewingFeedbackId
        description: viewing feedback id
      responses:
        200:
          description: OK
      tags:
      - Edit
      - That
      - Feedbacka
      - Viewing
      - Was
      - Notified
      - To
      - Vendor
  /api/viewing/{viewingFeedbackId}/editfeedbackreviewed:
    put:
      summary: Edit whether the vendor feedback for the viewing has been reviewed.
      description: Edit whether the vendor feedback for the viewing has been reviewed..
      operationId: Viewing_EditFeedbackReviewedByviewingFeedbackIdBymarkAsReviewed
      x-api-path-slug: apiviewingviewingfeedbackideditfeedbackreviewed-put
      parameters:
      - in: query
        name: markAsReviewed
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: viewingFeedbackId
        description: viewing feedback id
      responses:
        200:
          description: OK
      tags:
      - Edit
      - Whether
      - Vendor
      - Feedbackthe
      - Viewing
      - Has
      - Been
      - Reviewed
  /api/viewing/{id}/recordslotapproval/{viewingSlotId}:
    put:
      summary: Set approval status of viewing slot on multi viewing appointment
      description: Set approval status of viewing slot on multi viewing appointment.
      operationId: Viewing_RecordViewingSlotApprovalByidByviewingSlotIdBystatus
      x-api-path-slug: apiviewingidrecordslotapprovalviewingslotid-put
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: status
      - in: path
        name: viewingSlotId
      responses:
        200:
          description: OK
      tags:
      - Set
      - Approval
      - Status
      - Of
      - Viewing
      - Slot
      - "On"
      - Multi
      - Viewing
      - Appointment
  /api/viewing/{id}/delete:
    delete:
      summary: Endpoint to complete the multi viewing container once individual appointments
        have been booked.
      description: Endpoint to complete the multi viewing container once individual
        appointments have been booked..
      operationId: Viewing_CompleteMultiViewingBookingByid
      x-api-path-slug: apiviewingiddelete-delete
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Endpoint
      - To
      - Complete
      - Multi
      - Viewing
      - Container
      - Once
      - Individual
      - Appointments
      - Have
      - Been
      - Booked
  /api/Viewing/{id}:
    get:
      summary: Get an Viewing by its id.
      description: Get an viewing by its id..
      operationId: Viewing_GetByid
      x-api-path-slug: apiviewingid-get
      parameters:
      - in: path
        name: id
        description: The id of the Viewing to get
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Viewing
      - By
      - Its
      - Id
    delete:
      summary: Cancel a viewing appointment by id if it exists.
      description: Cancel a viewing appointment by id if it exists..
      operationId: Viewing_DeleteByidBycancelAppointmentDataContract
      x-api-path-slug: apiviewingid-delete
      parameters:
      - in: body
        name: cancelAppointmentDataContract
        description: The cancellation details, including reason of cancellation
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: the viewing appointment id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Viewing
      - Appointment
      - By
      - Id
      - If
      - It
      - Exists
  /api/todo/assignleadstopredefinedteams:
    put:
      summary: Assign InboundLead Todos to the predefined neg teams. e.g. Sales Valuers,
        Sales Viewings, Lettings Viewings etc etc
      description: Assign inboundlead todos to the predefined neg teams. e.g. sales
        valuers, sales viewings, lettings viewings etc etc.
      operationId: DefaultToDo_AssignLeadsToPredefinedTeamsBytoDoId
      x-api-path-slug: apitodoassignleadstopredefinedteams-put
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: toDoId
      responses:
        200:
          description: OK
      tags:
      - Assign
      - InboundLead
      - Todos
      - To
      - Predefined
      - Neg
      - Teams
      - ""
      - E
      - G
      - ""
      - Sales
      - Valuers
      - ""
      - Sales
      - Viewings
      - ""
      - Lettings
      - Viewings
      - Etc
      - Etc
---