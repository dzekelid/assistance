---
swagger: "2.0"
x-collection-name: AXA Assistance
x-complete: 0
info:
  title: AXA Assistance Updates information related to the gas damage declaration
  description: Updates information related to the gas damage declaration
  version: 1.0.0
host: sandbox.api.axa-assistance.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /assistance/version:
    get:
      summary: Provide basic details about the current deployed version of the assistance
        API
      description: Provide basic details about the current deployed version of the
        assistance API
      operationId: getAssistanceVersion
      x-api-path-slug: assistanceversion-get
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Provide
      - basic
      - detailAssistance
      - about
      - the
      - current
      - deployed
      - version
      - of
      - the
      - assistance
      - API
  /information/version:
    get:
      summary: Provide basic details about the current deployed version of the information
        API
      description: Provide basic details about the current deployed version of the
        information API
      operationId: getInformationVersion
      x-api-path-slug: informationversion-get
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Provide
      - basic
      - detailAssistance
      - about
      - the
      - current
      - deployed
      - version
      - of
      - the
      - information
      - API
  /insurance/version:
    get:
      summary: Provide basic details about the current deployed version of the insurance
        API
      description: Provide basic details about the current deployed version of the
        insurance API
      operationId: getInsuranceVersion
      x-api-path-slug: insuranceversion-get
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Provide
      - basic
      - detailAssistance
      - about
      - the
      - current
      - deployed
      - version
      - of
      - the
      - insurance
      - API
  /network/version:
    get:
      summary: Provide basic details about the current deployed version of the network
        API
      description: Provide basic details about the current deployed version of the
        network API
      operationId: getNetworkVersion
      x-api-path-slug: networkversion-get
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Provide
      - basic
      - detailAssistance
      - about
      - the
      - current
      - deployed
      - version
      - of
      - the
      - network
      - API
  /ondemand/version:
    get:
      summary: Provide basic details about the current deployed version of the on
        demand API
      description: Provide basic details about the current deployed version of the
        on demand API
      operationId: getOndemandVersion
      x-api-path-slug: ondemandversion-get
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Provide
      - basic
      - detailAssistance
      - about
      - the
      - current
      - deployed
      - version
      - of
      - the
      - "on"
      - demand
      - API
  /sales/version:
    get:
      summary: Provide basic details about the current deployed version of the sales
        API
      description: Provide basic details about the current deployed version of the
        sales API
      operationId: getSalesVersion
      x-api-path-slug: salesversion-get
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Provide
      - basic
      - detailAssistance
      - about
      - the
      - current
      - deployed
      - version
      - of
      - the
      - saleAssistance
      - API
  /service/version:
    get:
      summary: Provide basic details about the current deployed version of the service
        API
      description: Provide basic details about the current deployed version of the
        service API
      operationId: getServiceVersion
      x-api-path-slug: serviceversion-get
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Provide
      - basic
      - detailAssistance
      - about
      - the
      - current
      - deployed
      - version
      - of
      - the
      - service
      - API
  /user/version:
    get:
      summary: Provide basic details about the current deployed version of the User
        API
      description: Provide basic details about the current deployed version of the
        User API
      operationId: getUserVersion
      x-api-path-slug: userversion-get
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Provide
      - basic
      - detailAssistance
      - about
      - the
      - current
      - deployed
      - version
      - of
      - the
      - User
      - API
  /assistance/v1/home/cases:
    get:
      summary: Gets details of cases
      description: Gets details of cases
      operationId: getAssistanceV1HomeCases
      x-api-path-slug: assistancev1homecases-get
      parameters:
      - in: query
        name: declaration_id
        description: ID of the declaration which has trigger the cases
      - in: query
        name: lastname
        description: Lastname of the person associated to the case
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - detailAssistance
      - of
      - cases
  /information/v1/countries/alerts:
    get:
      summary: Retrieve the latest alerts worldwide
      description: Retrieve the latest alerts worldwide
      operationId: getInformationV1CountriesAlerts
      x-api-path-slug: informationv1countriesalerts-get
      parameters:
      - in: header
        name: accept-language
        description: Language/Country
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Retrieve
      - the
      - latest
      - alertAssistance
      - worldwide
  /information/vexp/roadside/workshops:
    get:
      summary: Gets list of nearest workshops.
      description: Gets list of nearest workshops.
      operationId: getInformationVexpRoadsideWorkshops
      x-api-path-slug: informationvexproadsideworkshops-get
      parameters:
      - in: query
        name: latitude
        description: Latitude of the location around which to search, latitude to
          be provided in WGS84 format
      - in: query
        name: longitude
        description: Longitude of the location around which to search, longitude to
          be provided in WGS84 format
      - in: query
        name: radius
        description: Maximum distance around
      - in: query
        name: radius_unit
        description: Unit of radius, ISO-20022 Unit Of Measure 2 Code (required if
          radius is provided)
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - list
      - of
      - nearest
      - workshops.
  /network/v1/medical_providers/availabilities:
    get:
      summary: Gets the availabilities of medical providers.
      description: Gets the availabilities of medical providers.
      operationId: getNetworkV1Medical_providersAvailabilities
      x-api-path-slug: networkv1medical-providersavailabilities-get
      parameters:
      - in: query
        name: end_date
        description: End date and time of the availability search - UTC datetime,
          RFC3339 format (YYYY-MM-DDTHH:mmZ)
      - in: query
        name: start_date
        description: Beginning date and time of the availability search - UTC datetime,
          RFC3339 format (YYYY-MM-DDTHH:mmZ)
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - the
      - availabilitieAssistance
      - of
      - medical
      - providers.
  /network/vexp/roadside_providers/{provider_id}:
    get:
      summary: Gets information of roadside provider.
      description: Gets information of roadside provider.
      operationId: getNetworkVexpRoadside_providersProvider_id
      x-api-path-slug: networkvexproadside-providersprovider-id-get
      parameters:
      - in: path
        name: provider_id
        description: Provider unique id
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - information
      - of
      - roadside
      - provider.
  /ondemand/v1/medical_providers/kinds:
    get:
      summary: 'Retrieve all medical provider kinds available for search (Ex: pharmacy,
        hospital ...)'
      description: 'Retrieve all medical provider kinds available for search (Ex:
        pharmacy, hospital ...)'
      operationId: getOndemandV1Medical_providersKinds
      x-api-path-slug: ondemandv1medical-providerskinds-get
      parameters:
      - in: header
        name: accept-language
        description: Language/Country
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Retrieve
      - all
      - medical
      - provider
      - kindAssistance
      - availablesearch
      - '(Ex:'
      - pharmacy
      - ""
      - hospital
      - '...)'
  /ondemand/v1/medical_providers/specialities:
    get:
      summary: 'Retrieve all medical provider specialities available for search (Ex:
        cardiology, dentist ...)'
      description: 'Retrieve all medical provider specialities available for search
        (Ex: cardiology, dentist ...)'
      operationId: getOndemandV1Medical_providersSpecialities
      x-api-path-slug: ondemandv1medical-providersspecialities-get
      parameters:
      - in: header
        name: accept-language
        description: Language/Country
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Retrieve
      - all
      - medical
      - provider
      - specialitieAssistance
      - availablesearch
      - '(Ex:'
      - cardiology
      - ""
      - dentist
      - '...)'
  /service/v1/medical_consultations/{medical_consultation_id}:
    get:
      summary: Provides detail of a medical consultation
      description: Provides detail of a medical consultation
      operationId: getServiceV1Medical_consultationsMedical_consultation_id
      x-api-path-slug: servicev1medical-consultationsmedical-consultation-id-get
      parameters:
      - in: path
        name: medical_consultation_id
        description: ID of the medical consultation
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - ProvideAssistance
      - detail
      - ofmedical
      - consultation
  /service/vexp/roadside/assignments/{assignment_id}:
    get:
      summary: Gets assignment information.
      description: Gets assignment information.
      operationId: getServiceVexpRoadsideAssignmentsAssignment_id
      x-api-path-slug: servicevexproadsideassignmentsassignment-id-get
      parameters:
      - in: path
        name: assignment_id
        description: Assignment unique identifier
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - assignment
      - information.
  /sales/v1/individual/car_rental/certificates/{certificate_id}:
    get:
      summary: Gets the car rental certificate details.
      description: Gets the car rental certificate details.
      operationId: getSalesV1IndividualCar_rentalCertificatesCertificate_id
      x-api-path-slug: salesv1individualcar-rentalcertificatescertificate-id-get
      parameters:
      - in: header
        name: accept-language
        description: Accepted language, IANA language codification
      - in: path
        name: certificate_id
        description: Certificate unique identifier
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - the
      - car
      - rental
      - certificate
      - details.
  /sales/v1/individual/travel/certificates/{certificate_id}:
    get:
      summary: Gets the travel certificate details.
      description: Gets the travel certificate details.
      operationId: getSalesV1IndividualTravelCertificatesCertificate_id
      x-api-path-slug: salesv1individualtravelcertificatescertificate-id-get
      parameters:
      - in: header
        name: accept-language
        description: Accepted language, IANA language codification
      - in: path
        name: certificate_id
        description: Certificate unique identifier
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - the
      - travel
      - certificate
      - details.
  /service/v1/medical_consultations/{medical_consultation_id}/prescriptions/{prescription_id}:
    get:
      summary: Provides detail of a prescription
      description: Provides detail of a prescription
      operationId: getServiceV1Medical_consultationsMedical_consultation_idPrescriptionsPrescription_id
      x-api-path-slug: servicev1medical-consultationsmedical-consultation-idprescriptionsprescription-id-get
      parameters:
      - in: path
        name: medical_consultation_id
        description: ID of the medical consultation
      - in: path
        name: prescription_id
        description: ID of the prescription
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - ProvideAssistance
      - detail
      - ofprescription
  /assistance/v1/home/electric_damage/declarations/{declaration_id}/policy_holders:
    get:
      summary: Gets the policy holders details for the electric damage
      description: Gets the policy holders details for the electric damage
      operationId: getAssistanceV1HomeElectric_damageDeclarationsDeclaration_idPolicy_holders
      x-api-path-slug: assistancev1homeelectric-damagedeclarationsdeclaration-idpolicy-holders-get
      parameters:
      - in: path
        name: declaration_id
        description: ID of the declaration
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - the
      - policy
      - holderAssistance
      - detailsthe
      - electric
      - damage
  /assistance/v1/home/gas_damage/declarations/{declaration_id}/policy_holders:
    get:
      summary: Gets the policy holders details for the gas damage
      description: Gets the policy holders details for the gas damage
      operationId: getAssistanceV1HomeGas_damageDeclarationsDeclaration_idPolicy_holders
      x-api-path-slug: assistancev1homegas-damagedeclarationsdeclaration-idpolicy-holders-get
      parameters:
      - in: path
        name: declaration_id
        description: ID of the declaration
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - the
      - policy
      - holderAssistance
      - detailsthe
      - gaAssistance
      - damage
  /assistance/v1/home/glaziery_damage/declarations/{declaration_id}/policy_holders:
    get:
      summary: Gets the information linked to the policy holder of the glaziery damage
        declaration
      description: Gets the information linked to the policy holder of the glaziery
        damage declaration
      operationId: getAssistanceV1HomeGlaziery_damageDeclarationsDeclaration_idPolicy_holders
      x-api-path-slug: assistancev1homeglaziery-damagedeclarationsdeclaration-idpolicy-holders-get
      parameters:
      - in: path
        name: declaration_id
        description: ID of the declaration
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - the
      - information
      - linked
      - to
      - the
      - policy
      - holder
      - of
      - the
      - glaziery
      - damage
      - Declarations
  /assistance/v1/home/home_appliance_damage/declarations/{declaration_id}/policy_holders:
    get:
      summary: Gets the information linked to the policy holder of the home appliance
        damage declaration
      description: Gets the information linked to the policy holder of the home appliance
        damage declaration
      operationId: getAssistanceV1HomeHome_appliance_damageDeclarationsDeclaration_idPolicy_holders
      x-api-path-slug: assistancev1homehome-appliance-damagedeclarationsdeclaration-idpolicy-holders-get
      parameters:
      - in: path
        name: declaration_id
        description: ID of the declaration
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - the
      - information
      - linked
      - to
      - the
      - policy
      - holder
      - of
      - the
      - home
      - appliance
      - damage
      - Declarations
  /assistance/v1/home/locksmithing_damage/declarations/{declaration_id}/policy_holders:
    get:
      summary: Gets the information linked to the policy holder of the locksmithing
        damage declaration
      description: Gets the information linked to the policy holder of the locksmithing
        damage declaration
      operationId: getAssistanceV1HomeLocksmithing_damageDeclarationsDeclaration_idPolicy_holders
      x-api-path-slug: assistancev1homelocksmithing-damagedeclarationsdeclaration-idpolicy-holders-get
      parameters:
      - in: path
        name: declaration_id
        description: ID of the declaration
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - the
      - information
      - linked
      - to
      - the
      - policy
      - holder
      - of
      - the
      - locksmithing
      - damage
      - Declarations
  /assistance/v1/home/water_damage/declarations/{declaration_id}/policy_holders:
    get:
      summary: Gets the information related to each the policy holder of the water
        damage declaration
      description: Gets the information related to each the policy holder of the water
        damage declaration
      operationId: getAssistanceV1HomeWater_damageDeclarationsDeclaration_idPolicy_holders
      x-api-path-slug: assistancev1homewater-damagedeclarationsdeclaration-idpolicy-holders-get
      parameters:
      - in: path
        name: declaration_id
        description: ID of the declaration
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - the
      - information
      - related
      - to
      - each
      - the
      - policy
      - holder
      - of
      - the
      - water
      - damage
      - Declarations
  /insurance/vexp/appliance/claims:
    post:
      summary: Requests to create a claim related to an appliance.
      description: Requests to create a claim related to an appliance.
      operationId: postInsuranceVexpApplianceClaims
      x-api-path-slug: insurancevexpapplianceclaims-post
      parameters:
      - in: header
        name: accept-language
        description: Accepted language, IANA language codification
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - RequestAssistance
      - to
      - createclaim
      - related
      - toappliance.
  /insurance/vexp/car_rental/claims:
    post:
      summary: Requests to create a claim related to a car rental.
      description: Requests to create a claim related to a car rental.
      operationId: postInsuranceVexpCar_rentalClaims
      x-api-path-slug: insurancevexpcar-rentalclaims-post
      parameters:
      - in: header
        name: accept-language
        description: Accepted language, IANA language codification
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - RequestAssistance
      - to
      - createclaim
      - related
      - tocar
      - rental.
  /insurance/vexp/corporate_liability/claims:
    post:
      summary: Requests to create a claim related to a corporate liability.
      description: Requests to create a claim related to a corporate liability.
      operationId: postInsuranceVexpCorporate_liabilityClaims
      x-api-path-slug: insurancevexpcorporate-liabilityclaims-post
      parameters:
      - in: header
        name: accept-language
        description: Accepted language, IANA language codification
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - RequestAssistance
      - to
      - createclaim
      - related
      - tocorporate
      - liability.
  /insurance/vexp/delayed_luggage/claims:
    post:
      summary: Requests to create a claim related to a delayed luggage.
      description: Requests to create a claim related to a delayed luggage.
      operationId: postInsuranceVexpDelayed_luggageClaims
      x-api-path-slug: insurancevexpdelayed-luggageclaims-post
      parameters:
      - in: header
        name: accept-language
        description: Accepted language, IANA language codification
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - RequestAssistance
      - to
      - createclaim
      - related
      - todelayed
      - luggage.
  /insurance/vexp/delayed_trip/claims:
    post:
      summary: Requests to create a claim related to a delayed trip.
      description: Requests to create a claim related to a delayed trip.
      operationId: postInsuranceVexpDelayed_tripClaims
      x-api-path-slug: insurancevexpdelayed-tripclaims-post
      parameters:
      - in: header
        name: accept-language
        description: Accepted language, IANA language codification
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - RequestAssistance
      - to
      - createclaim
      - related
      - todelayed
      - trip.
  /insurance/vexp/lost_baggage/claims:
    post:
      summary: Requests to create a claim related to a lost baggage.
      description: Requests to create a claim related to a lost baggage.
      operationId: postInsuranceVexpLost_baggageClaims
      x-api-path-slug: insurancevexplost-baggageclaims-post
      parameters:
      - in: header
        name: accept-language
        description: Accepted language, IANA language codification
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - RequestAssistance
      - to
      - createclaim
      - related
      - tolost
      - baggage.
  /insurance/vexp/missed_flight/claims:
    post:
      summary: Requests to create a claim related to a missed flight.
      description: Requests to create a claim related to a missed flight.
      operationId: postInsuranceVexpMissed_flightClaims
      x-api-path-slug: insurancevexpmissed-flightclaims-post
      parameters:
      - in: header
        name: accept-language
        description: Accepted language, IANA language codification
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - RequestAssistance
      - to
      - createclaim
      - related
      - tomissed
      - flight.
  /insurance/vexp/price_protection/claims:
    post:
      summary: Requests to create a claim related to a price protection.
      description: Requests to create a claim related to a price protection.
      operationId: postInsuranceVexpPrice_protectionClaims
      x-api-path-slug: insurancevexpprice-protectionclaims-post
      parameters:
      - in: header
        name: accept-language
        description: Accepted language, IANA language codification
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - RequestAssistance
      - to
      - createclaim
      - related
      - toprice
      - protection.
  /insurance/vexp/stolen_cash/claims:
    post:
      summary: Requests to create a claim related to a stolen cash.
      description: Requests to create a claim related to a stolen cash.
      operationId: postInsuranceVexpStolen_cashClaims
      x-api-path-slug: insurancevexpstolen-cashclaims-post
      parameters:
      - in: header
        name: accept-language
        description: Accepted language, IANA language codification
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - RequestAssistance
      - to
      - createclaim
      - related
      - tostolen
      - cash.
  /insurance/vexp/travel_accident/claims:
    post:
      summary: Requests to create a claim related to a travel accident.
      description: Requests to create a claim related to a travel accident.
      operationId: postInsuranceVexpTravel_accidentClaims
      x-api-path-slug: insurancevexptravel-accidentclaims-post
      parameters:
      - in: header
        name: accept-language
        description: Accepted language, IANA language codification
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - RequestAssistance
      - to
      - createclaim
      - related
      - totravel
      - accident.
  /insurance/vexp/trip/claims:
    post:
      summary: Requests to create a claim related to a trip.
      description: Requests to create a claim related to a trip.
      operationId: postInsuranceVexpTripClaims
      x-api-path-slug: insurancevexptripclaims-post
      parameters:
      - in: header
        name: accept-language
        description: Accepted language, IANA language codification
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - RequestAssistance
      - to
      - createclaim
      - related
      - totrip.
  /insurance/vexp/trip_cancellation/claims:
    post:
      summary: Requests to create a claim related to a trip cancellation.
      description: Requests to create a claim related to a trip cancellation.
      operationId: postInsuranceVexpTrip_cancellationClaims
      x-api-path-slug: insurancevexptrip-cancellationclaims-post
      parameters:
      - in: header
        name: accept-language
        description: Accepted language, IANA language codification
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - RequestAssistance
      - to
      - createclaim
      - related
      - totrip
      - cancellation.
  /service/vexp/roadside/assignments:
    post:
      summary: Creates new assignment.
      description: Creates new assignment.
      operationId: postServiceVexpRoadsideAssignments
      x-api-path-slug: servicevexproadsideassignments-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - CreateAssistance
      - new
      - assignment.
  /assistance/v1/home/gas_damage/declarations:
    post:
      summary: Creates a declaration for a gas damage
      description: Creates a declaration for a gas damage
      operationId: postAssistanceV1HomeGas_damageDeclarations
      x-api-path-slug: assistancev1homegas-damagedeclarations-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - CreatesDeclarationsa
      - gaAssistance
      - damage
  /sales/v1/individual/appliance/certificates:
    post:
      summary: Requests the activation of a certificate either to cover an appliance
        purchased or to extend the warranty period of an appliance purchased. At least
        one product_criteria has to be specified to identify the product to which
        to subscribe. This endpoint
      description: Requests the activation of a certificate either to cover an appliance
        purchased or to extend the warranty period of an appliance purchased. At least
        one product_criteria has to be specified to identify the product to which
        to subscribe. This endpoint
      operationId: postSalesV1IndividualApplianceCertificates
      x-api-path-slug: salesv1individualappliancecertificates-post
      parameters:
      - in: header
        name: accept-language
        description: Accepted language, IANA language codification
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - RequestAssistance
      - the
      - activation
      - ofcertificate
      - either
      - to
      - coverappliance
      - purchasedto
      - extend
      - the
      - warranty
      - period
      - ofappliance
      - purchased.
      - At
      - leastproduct_criteria
      - haAssistance
      - to
      - be
      - specified
      - to
      - identify
      - the
      - product
      - to
      - which
      - to
      - subscribe.
      - ThiAssistance
      - endpoint
  /sales/v1/individual/car_rental/certificates:
    post:
      summary: Requests the activation of a car rental certificate linked to a product.
        At least one product_criteria has to be specified to identify the product
        to which to subscribe. If the user already holds a certificate, this api will
        update its personal infor
      description: Requests the activation of a car rental certificate linked to a
        product. At least one product_criteria has to be specified to identify the
        product to which to subscribe. If the user already holds a certificate, this
        api will update its personal infor
      operationId: postSalesV1IndividualCar_rentalCertificates
      x-api-path-slug: salesv1individualcar-rentalcertificates-post
      parameters:
      - in: header
        name: accept-language
        description: Accepted language, IANA language codification
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - RequestAssistance
      - the
      - activation
      - ofcar
      - rental
      - certificate
      - linked
      - toproduct.
      - At
      - leastproduct_criteria
      - haAssistance
      - to
      - be
      - specified
      - to
      - identify
      - the
      - product
      - to
      - which
      - to
      - subscribe.
      - If
      - the
      - user
      - already
      - holdscertificate
      - ""
      - thiAssistance
      - api
      - will
      - update
      - itAssistance
      - personal
      - infor
  /sales/v1/individual/travel/certificates:
    post:
      summary: Requests the activation of a travel certificate linked to a product.
        At least one product_criteria has to be specified to identify the product
        to which to subscribe. If the user already holds a certificate, this api will
        update its personal informati
      description: Requests the activation of a travel certificate linked to a product.
        At least one product_criteria has to be specified to identify the product
        to which to subscribe. If the user already holds a certificate, this api will
        update its personal informati
      operationId: postSalesV1IndividualTravelCertificates
      x-api-path-slug: salesv1individualtravelcertificates-post
      parameters:
      - in: header
        name: accept-language
        description: Accepted language, IANA language codification
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - RequestAssistance
      - the
      - activation
      - oftravel
      - certificate
      - linked
      - toproduct.
      - At
      - leastproduct_criteria
      - haAssistance
      - to
      - be
      - specified
      - to
      - identify
      - the
      - product
      - to
      - which
      - to
      - subscribe.
      - If
      - the
      - user
      - already
      - holdscertificate
      - ""
      - thiAssistance
      - api
      - will
      - update
      - itAssistance
      - personal
      - informati
  /user/v1/identities/register/confirm/resend:
    post:
      summary: Resends the confirmation email to an identity account
      description: Resends the confirmation email to an identity account
      operationId: postUserV1IdentitiesRegisterConfirmResend
      x-api-path-slug: userv1identitiesregisterconfirmresend-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - ResendAssistance
      - the
      - confirmation
      - email
      - toidentity
      - account
  /assistance/v1/home/electric_damage/declarations/{declaration_id}/contacts:
    post:
      summary: Adds contact information of the electric damage declaration
      description: Adds contact information of the electric damage declaration
      operationId: postAssistanceV1HomeElectric_damageDeclarationsDeclaration_idContacts
      x-api-path-slug: assistancev1homeelectric-damagedeclarationsdeclaration-idcontacts-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: declaration_id
        description: ID of the declaration
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - contact
      - information
      - of
      - the
      - electric
      - damage
      - Declarations
  /assistance/v1/home/gas_damage/declarations/{declaration_id}/contacts:
    post:
      summary: Adds contact information of the gas damage declaration
      description: Adds contact information of the gas damage declaration
      operationId: postAssistanceV1HomeGas_damageDeclarationsDeclaration_idContacts
      x-api-path-slug: assistancev1homegas-damagedeclarationsdeclaration-idcontacts-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: declaration_id
        description: ID of the declaration
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - contact
      - information
      - of
      - the
      - gaAssistance
      - damage
      - Declarations
  /assistance/v1/home/gas_damage/declarations/{declaration_id}/confirm:
    post:
      summary: Gas declaration confirmation
      description: Gas declaration confirmation
      operationId: postAssistanceV1HomeGas_damageDeclarationsDeclaration_idConfirm
      x-api-path-slug: assistancev1homegas-damagedeclarationsdeclaration-idconfirm-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: declaration_id
        description: ID of the declaration
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - Declarations
      - confirmation
  /assistance/v1/home/gas_damage/declarations/{declaration_id}/close:
    post:
      summary: Gas declaration closure
      description: Gas declaration closure
      operationId: postAssistanceV1HomeGas_damageDeclarationsDeclaration_idClose
      x-api-path-slug: assistancev1homegas-damagedeclarationsdeclaration-idclose-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: declaration_id
        description: ID of the declaration
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - Declarations
      - closure
  /assistance/v1/home/glaziery_damage/declarations/{declaration_id}/confirm:
    post:
      summary: Confirms the need for assistance
      description: Confirms the need for assistance
      operationId: postAssistanceV1HomeGlaziery_damageDeclarationsDeclaration_idConfirm
      x-api-path-slug: assistancev1homeglaziery-damagedeclarationsdeclaration-idconfirm-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: declaration_id
        description: ID of the declaration
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - ConfirmAssistance
      - the
      - needassistance
  /assistance/v1/home/glaziery_damage/declarations/{declaration_id}/close:
    post:
      summary: Closes the declaration after an other fixing solution
      description: Closes the declaration after an other fixing solution
      operationId: postAssistanceV1HomeGlaziery_damageDeclarationsDeclaration_idClose
      x-api-path-slug: assistancev1homeglaziery-damagedeclarationsdeclaration-idclose-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: declaration_id
        description: ID of the declaration
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - CloseAssistance
      - the
      - Declarations
      - afterother
      - fixing
      - solution
  /assistance/v1/home/glaziery_damage/declarations/{declaration_id}/contacts:
    post:
      summary: Adds contact information of the glaziery damage declaration
      description: Adds contact information of the glaziery damage declaration
      operationId: postAssistanceV1HomeGlaziery_damageDeclarationsDeclaration_idContacts
      x-api-path-slug: assistancev1homeglaziery-damagedeclarationsdeclaration-idcontacts-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: declaration_id
        description: ID of the declaration
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - contact
      - information
      - of
      - the
      - glaziery
      - damage
      - Declarations
  /assistance/v1/home/home_appliance_damage/declarations/{declaration_id}/confirm:
    post:
      summary: Confirms the need for assistance
      description: Confirms the need for assistance
      operationId: postAssistanceV1HomeHome_appliance_damageDeclarationsDeclaration_idConfirm
      x-api-path-slug: assistancev1homehome-appliance-damagedeclarationsdeclaration-idconfirm-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: declaration_id
        description: ID of the declaration
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - ConfirmAssistance
      - the
      - needassistance
  /assistance/v1/home/home_appliance_damage/declarations/{declaration_id}/contacts:
    post:
      summary: Adds contact information of the home appliance damage declaration
      description: Adds contact information of the home appliance damage declaration
      operationId: postAssistanceV1HomeHome_appliance_damageDeclarationsDeclaration_idContacts
      x-api-path-slug: assistancev1homehome-appliance-damagedeclarationsdeclaration-idcontacts-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: declaration_id
        description: ID of the declaration
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - contact
      - information
      - of
      - the
      - home
      - appliance
      - damage
      - Declarations
  /assistance/v1/home/home_appliance_damage/declarations/{declaration_id}/close:
    post:
      summary: Closes the declaration after an other fixing solution
      description: Closes the declaration after an other fixing solution
      operationId: postAssistanceV1HomeHome_appliance_damageDeclarationsDeclaration_idClose
      x-api-path-slug: assistancev1homehome-appliance-damagedeclarationsdeclaration-idclose-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: declaration_id
        description: ID of the request
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - CloseAssistance
      - the
      - Declarations
      - afterother
      - fixing
      - solution
  /assistance/v1/home/locksmithing_damage/declarations/{declaration_id}/close:
    post:
      summary: Closes the declaration after an other fixing solution
      description: Closes the declaration after an other fixing solution
      operationId: postAssistanceV1HomeLocksmithing_damageDeclarationsDeclaration_idClose
      x-api-path-slug: assistancev1homelocksmithing-damagedeclarationsdeclaration-idclose-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: declaration_id
        description: ID of the declaration
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - CloseAssistance
      - the
      - Declarations
      - afterother
      - fixing
      - solution
  /assistance/v1/home/locksmithing_damage/declarations/{declaration_id}/confirm:
    post:
      summary: Confirms the need for assistance
      description: Confirms the need for assistance
      operationId: postAssistanceV1HomeLocksmithing_damageDeclarationsDeclaration_idConfirm
      x-api-path-slug: assistancev1homelocksmithing-damagedeclarationsdeclaration-idconfirm-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: declaration_id
        description: ID of the declaration
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - ConfirmAssistance
      - the
      - needassistance
  /assistance/v1/home/locksmithing_damage/declarations/{declaration_id}/contacts:
    post:
      summary: Adds contact information of the locksmithing damage declaration
      description: Adds contact information of the locksmithing damage declaration
      operationId: postAssistanceV1HomeLocksmithing_damageDeclarationsDeclaration_idContacts
      x-api-path-slug: assistancev1homelocksmithing-damagedeclarationsdeclaration-idcontacts-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: declaration_id
        description: ID of the declaration
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - contact
      - information
      - of
      - the
      - locksmithing
      - damage
      - Declarations
  /assistance/v1/home/water_damage/declarations/{declaration_id}/contacts:
    post:
      summary: Adds contact information of the water damage declaration
      description: Adds contact information of the water damage declaration
      operationId: postAssistanceV1HomeWater_damageDeclarationsDeclaration_idContacts
      x-api-path-slug: assistancev1homewater-damagedeclarationsdeclaration-idcontacts-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: declaration_id
        description: ID of the declaration
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - contact
      - information
      - of
      - the
      - water
      - damage
      - Declarations
  /assistance/v1/home/water_damage/declarations/{declaration_id}/close:
    post:
      summary: Closes the declaration after an other fixing solution
      description: Closes the declaration after an other fixing solution
      operationId: postAssistanceV1HomeWater_damageDeclarationsDeclaration_idClose
      x-api-path-slug: assistancev1homewater-damagedeclarationsdeclaration-idclose-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: declaration_id
        description: ID of the declaration
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - CloseAssistance
      - the
      - Declarations
      - afterother
      - fixing
      - solution
  /assistance/v1/home/water_damage/declarations/{declaration_id}/confirm:
    post:
      summary: Confirms the need for assistance
      description: Confirms the need for assistance
      operationId: postAssistanceV1HomeWater_damageDeclarationsDeclaration_idConfirm
      x-api-path-slug: assistancev1homewater-damagedeclarationsdeclaration-idconfirm-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: declaration_id
        description: ID of the declaration
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - ConfirmAssistance
      - the
      - needassistance
  /service/v1/medical_consultations/{medical_consultation_id}/prescriptions/{prescription_id}/send:
    post:
      summary: Sends a prescription to its recipient
      description: Sends a prescription to its recipient
      operationId: postServiceV1Medical_consultationsMedical_consultation_idPrescriptionsPrescription_idSend
      x-api-path-slug: servicev1medical-consultationsmedical-consultation-idprescriptionsprescription-idsend-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: medical_consultation_id
        description: ID of the medical consultation
      - in: path
        name: prescription_id
        description: ID of the prescription
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Sendsprescription
      - to
      - itAssistance
      - recipient
  /assistance/v1/home/electric_damage/declarations/{declaration_id}:
    patch:
      summary: Updates information related to the electric damage declaration
      description: Updates information related to the electric damage declaration
      operationId: patchAssistanceV1HomeElectric_damageDeclarationsDeclaration_id
      x-api-path-slug: assistancev1homeelectric-damagedeclarationsdeclaration-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: declaration_id
        description: ID of the declaration
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - information
      - related
      - to
      - the
      - electric
      - damage
      - Declarations
  /assistance/v1/home/gas_damage/declarations/{declaration_id}:
    patch:
      summary: Updates information related to the gas damage declaration
      description: Updates information related to the gas damage declaration
      operationId: patchAssistanceV1HomeGas_damageDeclarationsDeclaration_id
      x-api-path-slug: assistancev1homegas-damagedeclarationsdeclaration-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: declaration_id
        description: ID of the declaration
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - information
      - related
      - to
      - the
      - gaAssistance
      - damage
      - Declarations
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