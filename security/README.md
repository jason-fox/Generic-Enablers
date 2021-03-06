# Security Access and API Management

In FIWARE we offer some services and tools to allow you to manage authentication and authorization in your applications
and backend services. If you want to manage identity in your application without developing your own mechanisms, you can
offer your users the possibility to log in to your app using their FIWARE Accounts.

This is possible thanks to the OAuth2 protocol and Keyrock, the Identity Manager component of FIWARE. In the same way
that you usually log in to some services using your Twitter or Facebook account, your users will use their FIWARE
accounts to access your service. But this is only the first step, because you can also secure your backends using FIWARE
Account. If your service or GE has a REST API that can be accessed from Internet, probably you want to manage the access
to the resources. For instance, you can allow the access only to the users that have a FIWARE account.

To learn more about Security Access and API Management, check out the
[documentation](https://fiwaretourguide.readthedocs.io/en/latest/security/introduction/)

## Keyrock

[![](https://nexus.lab.fiware.org/repository/raw/public/badges/chapters/security.svg)](./README.md)
![License](https://img.shields.io/github/license/ging/fiware-idm.svg)
![](https://img.shields.io/github/release-date/ging/fiware-idm.svg)
![](https://img.shields.io/github/commits-since/ging/fiware-idm/latest.svg)

| :octocat: [Git Repository](https://github.com/ging/fiware-idm) | :whale: [Docker Hub](https://hub.docker.com/r/fiware/idm/) | :books: [Documentation](https://fiware-idm.readthedocs.io/en/latest/) | :mortar_board: [Academy](https://fiware-academy.readthedocs.io/en/latest/security/keyrock) | :dart: [Roadmap](https://github.com/ging/fiware-idm/blob/master/roadmap.md) |
| -------------------------------------------------------------- | ---------------------------------------------------------- | --------------------------------------------------------------------- | ------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------- |


### What is Keyrock?

Identity Management covers a number of aspects involving users' access to networks, services and applications, including
secure and private authentication from users to devices, networks and services, authorization & trust management, user
profile management, privacy-preserving disposition of personal data, Single Sign-On (SSO) to service domains and
Identity Federation towards applications. The Identity Manager is the central component that provides a bridge between
IdM systems at connectivity-level and application-level. Furthermore, Identity Management is used for authorising
foreign services to access personal data stored in a secure environment. Hereby usually the owner of the data must give
consent to access the data; the consent-giving procedure also implies certain user authentication.

### Why use Keyrock?

Identity Management is key on any architecture. IdM offers tools for administrators to support the handling of user
lifecycle functions. It reduces the effort for account creation and management, as it supports the enforcement of
policies and procedures for user registration, user profile management and the modification of user accounts.
Administrators can quickly configure customized pages for the inclusion of different authentication providers,
registration of tenant applications with access to user profile data and the handling of error notifications.

For end users, the IdM provides a convenient solution for registering with applications since it gives them a means to
re-use attributes like address, email or others, thus allowing an easy and convenient management of profile information.
Users and administrators can rely on standardized solutions to allow user self-service features. In addition to
providing a native login, IdM supports the integration of multiple 3rd party authentication providers. Foremost, it
supports in a first step the configuration of preferred identity providers through the administrators. The use of 3rd
party IdMs lowers the entry barriers for a native user to register, since the user can link to her/his preferred IdM and
use this account for authentication. As it is possible to configure several applications that shall be linked to his
IdM, the main benefit for users is a single sign-on (SSO) to all these applications. The IdM offers hosted user profile
storage with specific user profile attributes. Applications do not have to run and manage their own persistent user data
storages, but instead, can use the IdM user profile storage as a Software as a Service (SaaS) offering.

The KeyRock Identity Management GEI complies with existing standards for user authentication and it provides access
information to services acting as a Single Sign-On platform. The KeyRock IdM is a free/open source software which code
can be found at Github: KeyRock source code It can be integrated with any development, specially with any Cloud service.
The installation guide can be found at the Github's wiki page: KeyRock installation guide and KeyRock User and
Programmers guide

## Wilma

[![](https://nexus.lab.fiware.org/repository/raw/public/badges/chapters/security.svg)](./README.md)
![License](https://img.shields.io/github/license/ging/fiware-pep-proxy.svg)
![](https://img.shields.io/github/release-date/ging/fiware-pep-proxy.svg)
![](https://img.shields.io/github/commits-since/ging/fiware-pep-proxy/latest.svg)

| :octocat: [Git Repository](https://github.com/ging/fiware-pep-proxy) | :whale: [Docker Hub](https://hub.docker.com/r/fiware/pep-proxy/) | :books: [Documentation](https://fiware-pep-proxy.rtfd.io/) | :mortar_board: [Academy](https://fiware-academy.readthedocs.io/en/latest/security/wilma) | :dart: [Roadmap](https://github.com/ging/fiware-pep-proxy/blob/master/roadmap.md) |
| -------------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------- | ---------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |


### What is Wilma?

You get the reference implementation of PEP Proxy Generic Enabler. Thanks to this component and together with Identity
Management and Authorization PDP GEs, you will add authentication and authorization security to your backend
applications. Thus, only FIWARE users will be able to access your GEs or REST services. But you will be able also to
manage specific permissions and policies to your resources allowing different access levels to your users.

### Why use Wilma?

Wilma is the reference implementation of this Generic Enabler because it is completely integrated with the FIWARE
ecosystem and specifically with FIWARE account. It is thought to work with OAuth2 and XACML protocols, the standards for
authentication and authorization chosen in FIWARE. Furthermore, this is the component that every GEis are including on
top of their REST APIs so it is tested and used in many different scenarios.

## Authzforce

[![](https://nexus.lab.fiware.org/repository/raw/public/badges/chapters/security.svg)](./README.md)
![License](https://img.shields.io/github/license/authzforce/server.svg)
![](https://img.shields.io/github/release-date/authzforce/server.svg)
![](https://img.shields.io/github/commits-since/authzforce/server/latest.svg)

| :octocat: [Git Repository](https://github.com/authzforce/server) | :whale: [Docker Hub](https://hub.docker.com/r/authzforce/server/) | :books: [Documentation](https://authzforce-ce-fiware.rtfd.io/) | :mortar_board: [Academy](https://fiware-academy.readthedocs.io/en/latest/security/authzforce) | :dart: [Roadmap](https://github.com/authzforce/server/blob/develop/ROADMAP.md) |
| ---------------------------------------------------------------- | ----------------------------------------------------------------- | -------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------ |


### What is Authzforce?

You get the reference implementation of the Authorization PDP Generic Enabler (formerly called Access Control GE).
Indeed, as mandated by the GE specification, this implementation provides an API to get authorization decisions based on
authorization policies, and authorization requests from PEPs. The API follows the REST architecture style, and complies
with XACML v3.0. XACML (eXtensible Access Control Markup Language) is a OASIS standard for authorization policy format
and evaluation logic, as well as for the authorization decision request/response format. The PDP (Policy Decision Point)
and the PEP (Policy Enforcement Point) terms are defined in the XACML standard. This GEri plays the role of a PDP.

To fulfill the XACML architecture, you may need a PEP (Policy Enforcement Point) to protect your application, which is
not provided here. For REST APIs, we recommend you use the PEP Proxy by UPM available in the catalogue.

### Why use Authzforce?

Providing authorization for your application is a must for security reasons. However, it is always a complex part to
implement, especially for non-security developers, because it involves advanced security concepts (Identity-based, RBAC,
ABAC, etc.). Most developers embed the authorization logic within the application code, which makes it hard to maintain,
evolve and integrate with external services providing extra authorization attributes. In this regard, the Authorization
PDP helps you externalize the authorization logic and take advantage of flexible and standard-compliant Attribute-Based
Access Control features. Combined with the Identity Management GE and the PEP proxy, this gives you a comprehensive
access control solution for your application.

The Authorization PDP specification defines a RESTful API of an Authorization Policy Decision Point (PDP) compliant with
the OASIS XACML standard. More specifically, it defines RESTful interfaces for: Managing XACML-compliant authorization
policies; Requesting authorization decisions based on those policies, in a XACML-compliant request-response format.

<a name="apinf"/>

## :seedling: APInf (Incubated)

[![](https://nexus.lab.fiware.org/repository/raw/public/badges/chapters/security.svg)](./README.md)
![License](https://img.shields.io/github/license/apinf/platform.svg)
![](https://img.shields.io/github/release-date/apinf/platform.svg)
![](https://img.shields.io/github/commits-since/apinf/platform/latest.svg)

| :octocat: [Git Repository](https://github.com/apinf/platform) | :whale: [Docker Hub](https://hub.docker.com/u/apinf/platform) | :books: [Documentation](https://apinf-fiware.readthedocs.io/en/latest/) | :page_facing_up: [Site](https://apinf.io/) | :mortar_board: [Academy](https://fiware-academy.readthedocs.io/en/latest/data-publication/apinf) |
| ------------------------------------------------------------- | ------------------------------------------------------------- | ----------------------------------------------------------------------- | ------------------------------------------ | ------------------------------------------------------------------------------------------------ |


### What is APInf?

The APInf API Management Framework is a Smart City orchestrator to be used together with other FIWARE enablers. APInf
integrates with FIWARE core technologies, such as [Identity Management](https://fiware-idm.readthedocs.io/en/latest/),
[NGSI v2](https://swagger.lab.fiware.org/?url=https://raw.githubusercontent.com/Fiware/specifications/master/OpenAPI/ngsiv2/ngsiv2-openapi.json)
and [Business API Ecosystem](https://business-api-ecosystem.rtfd.io/) along with [API Umbrella](https://apiumbrella.io/)
to offer a comprehensive toolset to let various API Owners to run business with their APIs. Public market place is one
of the essential GUI tools to help API Owners to reach their customer with the showcase.

The APInf API Management Framework is a highly extendable and can bring huge benefits to managed APIs - such as NGSI
based interfaces like FIWARE Context Broker instances. This extends opportunities to setup a complete IoT cloud for
Smart Cities using FIWARE technologies alone. Both right-time data and historical data will be available for software
developers to build Smart Applications.

### Why use APInf?

The APInf API Management Framework is a central part of the FIWARE platform combining with other Generic Enablers in an
offering a dashboard for all application developers. The business tools of the framework help API Owners to run their
API business. This helps cities to distribute digital technology in small pieces in order to let local small software
companies to attend in building the services to their home city. The support is close and this approach creates jobs for
local people, which in turn generate move tax money for the city to develop better digital services to the citizens.

<a name="fiware-true-connector"/>

## :seedling: FIWARE TRUE Connector (Incubated)

[![](https://nexus.lab.fiware.org/repository/raw/public/badges/chapters/security.svg)](./README.md)
![License](https://img.shields.io/github/license/Engineering-Research-and-Development/fiware-true-connector.svg)
![](https://img.shields.io/github/release-date/Engineering-Research-and-Development/fiware-true-connector.svg)
![](https://img.shields.io/github/commits-since/Engineering-Research-and-Development/fiware-true-connector/latest.svg)

| :octocat: [Git Repository](https://github.com/Engineering-Research-and-Development/fiware-true-connector) | :whale: [Docker Hub](https://github.com/Engineering-Research-and-Development/fiware-true-connector/blob/master/docs/docker_readme.md) | :books: [Documentation](https://fiware-true-connector.readthedocs.io/) |
| --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------- |


### What is the FIWARE TRUE Connector?

FIWARE TRUE Connector is a connector for the [International Data Spaces](https://internationaldataspaces.org/) (IDS)
ecosystem. FIWARE TRUE Connector enables trusted data exchange in order to be active part of an IDS Ecosystem, a virtual
data space leveraging existing standards and technologies, as well as governance models well-accepted in the data
economy, to facilitate secure and standardized data exchange and data linkage in a trusted business ecosystem. The
connector is compliant with the latest IDS specifications and can be easily customized to fit a wide spread of scenarios
thanks to the internal separation of Execution Core Container and Data App.

It is integrable with a lot of existing IDS services and totally configurable in terms of internal/external data format
(multipart/mixed, multipart/form, http-header) and protocols (HTTP, HTTPS, Web Socket over HTTPS, IDSCPv2).

### Why use the FIWARE TRUE Connector?

Trusted data exchange underpins data sovereignty, and allows users to pass context data between systems whilst limiting
the degree to which third-parties are able to use and receive the data.

IDSA envisages trusted data exchange taking place through federated entities, that are globally compliant with the
certification requirements defined by IDSA itself. The use of the connector allows data providers and consumers to join
these federated networks, or data spaces.

<a name="steeskin-pep"/>

## :seedling: Steelskin PEP (Incubated)

[![](https://nexus.lab.fiware.org/repository/raw/public/badges/chapters/security.svg)](./README.md)
![License](https://img.shields.io/github/license/telefonicaid/fiware-pep-steelskin.svg)
![](https://img.shields.io/github/release-date/telefonicaid/fiware-pep-steelskin.svg)
![](https://img.shields.io/github/commits-since/telefonicaid/fiware-pep-steelskin/latest.svg)

| :octocat: [Git Repository](https://github.com/telefonicaid/fiware-pep-steelskin) | :whale: [Docker Hub](https://hub.docker.com/r/telefonicaiot/fiware-pep-steelskin) | :books: [Documentation](https://github.com/telefonicaid/fiware-pep-steelskin#README.md) |
| -------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |


### What is Steelskin PEP?

Steelskin is a proxy meant to secure independent microservices such as FIWARE components, by intercepting every request
sent to the componen and validating it against an Access Control component. This validation is based in several pieces
of data:

-   `User token`: comes from the OAuth authorization server and is taken from the x-auth-token header.
-   `ServiceId`: is read from the fiware-service header and identifies the protected component.
-   `SubserviceId`: is read from the fiware-servicepath header and identifies further divisions of the service.
-   `Action`: the PEP guess the action for a particular request by checking the path or inspecting the body. The logic
    for performing such actions depends on the component that is being secured, so the PEP will need a plugin for each
    of this components.

### Why use Steelskin PEP?

A PEP Proxy lies in front of a secured resource and is an endpoint found at "well-known" public location. It serves as a
gatekeeper for resource access. Users or other actors must supply sufficient information to the PEP Proxy to allow their
request to succeed and pass through the PEP proxy. The PEP proxy then passes the request on to the real location of the
secured resource itself.

<a name="keypass"/>
    
## :seedling: Keypass (Incubated)

[![](https://nexus.lab.fiware.org/repository/raw/public/badges/chapters/security.svg)](./README.md)
![License](https://img.shields.io/github/license/telefonicaid/fiware-keypass.svg)
![](https://img.shields.io/github/release-date/telefonicaid/fiware-keypass.svg)
![](https://img.shields.io/github/commits-since/telefonicaid/fiware-keypass/latest.svg)

| :octocat: [Git Repository](https://github.com/telefonicaid/fiware-keypass) | :whale: [Docker Hub](https://hub.docker.com/r/telefonicaiot/fiware-keypass) | :books: [Documentation](telefonicaid/fiware-keypass#readme.md) |
| -------------------------------------------------------------------------- | --------------------------------------------------------------------------- | -------------------------------------------------------------- |


### What is Keypass?

Keypass is multi-tenant XACML server with PAP (Policy Administration Point) and PDP (Policy Decision Point)
capabilities.

### Why use Keypass?

The PDP is an adjudicator which checks whether the headers and other information found within the request permit the
user access to a resource or resources. XACML is a common standard for defining the rules of access and allowing
modification on the fly. The PAP allows users to set up roles, permissions etc. which underpin the ruleset of the PDP
creating a flexible security framework which can be applied to any microservice.

<a name="keystone-scim"/>

## :seedling: Keystone SCIM (Incubated)

[![](https://nexus.lab.fiware.org/repository/raw/public/badges/chapters/security.svg)](./README.md)
![License](https://img.shields.io/github/license/telefonicaid/fiware-keystone-scim.svg)
![](https://img.shields.io/github/last-commit/telefonicaid/fiware-keystone-scim)
![](https://img.shields.io/github/tag/telefonicaid/fiware-keystone-scim.svg)

| :octocat: [Git Repository](https://github.com/telefonicaid/fiware-keystone-scim) | :books: [Documentation](https://github.com/telefonicaid/fiware-keystone-scim/README.md) |
| -------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |


### What is Keystone SCIM?

Keystone SCIM is an OpenStack Keystone extension that enables the management of User, Groups and Roles using SCIM v1.1
standard. As any Keystone extension, it's designed to be installed on top of an existing Keystone installation,
following Keystone recommendations for extensions.

### Why use Keystone SCIM?

The SCIM standard is a standard for automating the exchange of user identity information between identity domains, or IT
systems. The extension enables the usage of this standard to define users, goups and roles. It can be installed onto a
running Keystone installation and enhance the functionality of it.

<a name="keystone-spassword"/>
    
## :seedling: Keystone SPASSWORD (Incubated)

[![](https://nexus.lab.fiware.org/repository/raw/public/badges/chapters/security.svg)](./README.md)
![License](https://img.shields.io/github/license/telefonicaid/fiware-keystone-spassword.svg)
![](https://img.shields.io/github/last-commit/telefonicaid/fiware-keystone-spassword)
![](https://img.shields.io/github/tag/telefonicaid/fiware-keystone-spassword.svg)

| :octocat: [Git Repository](https://github.com/telefonicaid/fiware-keystone-spassword) | :whale: [Docker Hub](https://hub.docker.com/r/telefonicaiot/fiware-keystone-spassword) | :books: [Documentation](https://github.com/telefonicaid/fiware-keystone-spassword/README.md) |
| ------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |


### What is Keystone SPASSWORD?

Keystone SPASSWORD is an OpenStack Keystone extension that enables some extra security checks over user passwords, such
as ensuring the usage of strong passwords, expiration time for a password, number of bad login attempts before user
account became temporarily blocked, a recover procedure password, a second factor authentication (2FA) and so on.

### Why use Keystone SPASSWORD?

Additional security checks and features improve the security and usability of a system, SPASSWORD helps to reduce
development time by avoiding the need to implement and test bespoke secure system functions.
