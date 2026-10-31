# Aerones

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Aerones is a Latvian robotics company that performs wind turbine blade inspection, cleaning, coating, leading-edge repair and lightning-protection testing with cable-suspended robots and autonomous drones, operating onshore and offshore for owners and OEMs including NextEra, GE, Vestas, Enel and Siemens Gamesa. Its software side is the Operations Hub — a Django Ninja backend behind portal.aerones.com that publishes an unauthenticated OpenAPI 3.1.0 description (760 paths, 1,114 operations, 1,377 schemas) alongside a companion GraphQL schema (339 queries, 325 mutations, 4 subscriptions), covering turbines, blades, anomalies, robot sets, work orders, dispatch, projects, inspections and accounting. Authentication is Keycloak OIDC on sso.aerones.com (realm "aerones", client "operations-hub"). The contract is public; the data behind it is customer- and staff-gated, and Aerones publishes no developer program, SDKs, pricing or partner API documentation.

**Areas:** Company · Wind Energy · Renewable Energy · Robotics · Drones · Inspection · Field Service Management · Asset Management · Industrial · Energy · Maintenance · Latvia

## Aerones on APIs.io

Everything profiled for Aerones is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/aerones/](https://apis.io/providers/aerones/)** — or go straight to one of the APIs or properties below.

### APIs (193)

- [Aerones Operations Hub GraphQL API](https://apis.io/apis/aerones/aerones-operations-hub-graphql/) — The GraphQL surface of the Aerones Operations Hub, served at /graphql with anonymous introspection enabled and the full SDL published as text/plain at…
- [Aerones Accounting API](https://apis.io/apis/aerones/aerones-accounting-api/) — The accounting API from Aerones — 11 operation(s) for accounting.
- [Aerones Accounting.billing Statements API](https://apis.io/apis/aerones/aerones-accounting-billing-statements-api/) — The accounting.billing-statements API from Aerones — 2 operation(s) for accounting.billing-statements.
- [Aerones Accounting.netsuite Departments API](https://apis.io/apis/aerones/aerones-accounting-netsuite-departments-api/) — The accounting.netsuite-departments API from Aerones — 1 operation(s) for accounting.netsuite-departments.
- [Aerones Accounting.notes API](https://apis.io/apis/aerones/aerones-accounting-notes-api/) — The accounting.notes API from Aerones — 2 operation(s) for accounting.notes.
- [Aerones Accounting.sales Invoices API](https://apis.io/apis/aerones/aerones-accounting-sales-invoices-api/) — The accounting.sales-invoices API from Aerones — 2 operation(s) for accounting.sales-invoices.
- [Aerones Accounting.sales Order Lines API](https://apis.io/apis/aerones/aerones-accounting-sales-order-lines-api/) — The accounting.sales-order-lines API from Aerones — 2 operation(s) for accounting.sales-order-lines.
- [Aerones Accounting.sales Orders API](https://apis.io/apis/aerones/aerones-accounting-sales-orders-api/) — The accounting.sales-orders API from Aerones — 2 operation(s) for accounting.sales-orders.
- [Aerones Accounting.service Charges API](https://apis.io/apis/aerones/aerones-accounting-service-charges-api/) — The accounting.service-charges API from Aerones — 2 operation(s) for accounting.service-charges.
- [Aerones Active Workload API](https://apis.io/apis/aerones/aerones-active-workload-api/) — The active-workload API from Aerones — 5 operation(s) for active-workload.
- [Aerones Auth API](https://apis.io/apis/aerones/aerones-auth-api/) — The auth API from Aerones — 4 operation(s) for auth.
- [Aerones Bamboohr.employees API](https://apis.io/apis/aerones/aerones-bamboohr-employees-api/) — The bamboohr.employees API from Aerones — 1 operation(s) for bamboohr.employees.
- [Aerones Bto.crew API](https://apis.io/apis/aerones/aerones-bto-crew-api/) — The bto.crew API from Aerones — 4 operation(s) for bto.crew.
- [Aerones Bto.travel Orders API](https://apis.io/apis/aerones/aerones-bto-travel-orders-api/) — The bto.travel-orders API from Aerones — 9 operation(s) for bto.travel-orders.
- [Aerones Commercial Offers API](https://apis.io/apis/aerones/aerones-commercial-offers-api/) — The commercial-offers API from Aerones — 2 operation(s) for commercial-offers.
- [Aerones Confluence API](https://apis.io/apis/aerones/aerones-confluence-api/) — The confluence API from Aerones — 1 operation(s) for confluence.
- [Aerones Core.anomalies API](https://apis.io/apis/aerones/aerones-core-anomalies-api/) — The core.anomalies API from Aerones — 14 operation(s) for core.anomalies.
- [Aerones Core.blade Diagrams API](https://apis.io/apis/aerones/aerones-core-blade-diagrams-api/) — The core.blade-diagrams API from Aerones — 2 operation(s) for core.blade-diagrams.
- [Aerones Core.business Regions API](https://apis.io/apis/aerones/aerones-core-business-regions-api/) — The core.business-regions API from Aerones — 1 operation(s) for core.business-regions.
- [Aerones Core.certificate Categories API](https://apis.io/apis/aerones/aerones-core-certificate-categories-api/) — The core.certificate-categories API from Aerones — 2 operation(s) for core.certificate-categories.
- [Aerones Core.certificate Expenses API](https://apis.io/apis/aerones/aerones-core-certificate-expenses-api/) — The core.certificate-expenses API from Aerones — 2 operation(s) for core.certificate-expenses.
- [Aerones Core.certificate Issuers API](https://apis.io/apis/aerones/aerones-core-certificate-issuers-api/) — The core.certificate-issuers API from Aerones — 2 operation(s) for core.certificate-issuers.
- [Aerones Core.certificate Offerings API](https://apis.io/apis/aerones/aerones-core-certificate-offerings-api/) — The core.certificate-offerings API from Aerones — 2 operation(s) for core.certificate-offerings.
- [Aerones Core.certificate Requirements API](https://apis.io/apis/aerones/aerones-core-certificate-requirements-api/) — The core.certificate-requirements API from Aerones — 4 operation(s) for core.certificate-requirements.
- [Aerones Core.certificates API](https://apis.io/apis/aerones/aerones-core-certificates-api/) — The core.certificates API from Aerones — 2 operation(s) for core.certificates.
- [Aerones Core.commercial Offers API](https://apis.io/apis/aerones/aerones-core-commercial-offers-api/) — The core.commercial-offers API from Aerones — 2 operation(s) for core.commercial-offers.
- [Aerones Core.component Models API](https://apis.io/apis/aerones/aerones-core-component-models-api/) — The core.component-models API from Aerones — 2 operation(s) for core.component-models.
- [Aerones Core.component Types API](https://apis.io/apis/aerones/aerones-core-component-types-api/) — The core.component-types API from Aerones — 1 operation(s) for core.component-types.
- [Aerones Core.countries API](https://apis.io/apis/aerones/aerones-core-countries-api/) — The core.countries API from Aerones — 1 operation(s) for core.countries.
- [Aerones Core.cross Sections API](https://apis.io/apis/aerones/aerones-core-cross-sections-api/) — The core.cross-sections API from Aerones — 2 operation(s) for core.cross-sections.
- [Aerones Core.currencies API](https://apis.io/apis/aerones/aerones-core-currencies-api/) — The core.currencies API from Aerones — 1 operation(s) for core.currencies.
- [Aerones Core.customer Locations API](https://apis.io/apis/aerones/aerones-core-customer-locations-api/) — The core.customer-locations API from Aerones — 1 operation(s) for core.customer-locations.
- [Aerones Core.customers.addresses API](https://apis.io/apis/aerones/aerones-core-customers-addresses-api/) — The core.customers.addresses API from Aerones — 2 operation(s) for core.customers.addresses.
- [Aerones Core.customers.anomaly Client Fields API](https://apis.io/apis/aerones/aerones-core-customers-anomaly-client-fields-api/) — The core.customers.anomaly-client-fields API from Aerones — 3 operation(s) for core.customers.anomaly-client-fields.
- [Aerones Core.customers API](https://apis.io/apis/aerones/aerones-core-customers-api/) — The core.customers API from Aerones — 3 operation(s) for core.customers.
- [Aerones Core.customers.bank Accounts API](https://apis.io/apis/aerones/aerones-core-customers-bank-accounts-api/) — The core.customers.bank-accounts API from Aerones — 2 operation(s) for core.customers.bank-accounts.
- [Aerones Core.customers.contacts API](https://apis.io/apis/aerones/aerones-core-customers-contacts-api/) — The core.customers.contacts API from Aerones — 2 operation(s) for core.customers.contacts.
- [Aerones Core.customers.locations API](https://apis.io/apis/aerones/aerones-core-customers-locations-api/) — The core.customers.locations API from Aerones — 2 operation(s) for core.customers.locations.
- [Aerones Core.customers.roles API](https://apis.io/apis/aerones/aerones-core-customers-roles-api/) — The core.customers.roles API from Aerones — 1 operation(s) for core.customers.roles.
- [Aerones Core.customers.turbines API](https://apis.io/apis/aerones/aerones-core-customers-turbines-api/) — The core.customers.turbines API from Aerones — 2 operation(s) for core.customers.turbines.
- [Aerones Core.customers.users API](https://apis.io/apis/aerones/aerones-core-customers-users-api/) — The core.customers.users API from Aerones — 2 operation(s) for core.customers.users.
- [Aerones Core.delay Categories API](https://apis.io/apis/aerones/aerones-core-delay-categories-api/) — The core.delay-categories API from Aerones — 2 operation(s) for core.delay-categories.
- [Aerones Core.delay Types API](https://apis.io/apis/aerones/aerones-core-delay-types-api/) — The core.delay-types API from Aerones — 2 operation(s) for core.delay-types.
- [Aerones Core.delays API](https://apis.io/apis/aerones/aerones-core-delays-api/) — The core.delays API from Aerones — 2 operation(s) for core.delays.
- [Aerones Core.erp Part Codes API](https://apis.io/apis/aerones/aerones-core-erp-part-codes-api/) — The core.erp-part-codes API from Aerones — 1 operation(s) for core.erp-part-codes.
- [Aerones Core.erp Parts API](https://apis.io/apis/aerones/aerones-core-erp-parts-api/) — The core.erp-parts API from Aerones — 2 operation(s) for core.erp-parts.
- [Aerones Core.file Entity Links API](https://apis.io/apis/aerones/aerones-core-file-entity-links-api/) — The core.file-entity-links API from Aerones — 2 operation(s) for core.file-entity-links.
- [Aerones Core.files API](https://apis.io/apis/aerones/aerones-core-files-api/) — The core.files API from Aerones — 6 operation(s) for core.files.
- [Aerones Core.item Categories API](https://apis.io/apis/aerones/aerones-core-item-categories-api/) — The core.item-categories API from Aerones — 1 operation(s) for core.item-categories.
- [Aerones Core.locations API](https://apis.io/apis/aerones/aerones-core-locations-api/) — The core.locations API from Aerones — 3 operation(s) for core.locations.
- [Aerones Core.manufacturers API](https://apis.io/apis/aerones/aerones-core-manufacturers-api/) — The core.manufacturers API from Aerones — 2 operation(s) for core.manufacturers.
- [Aerones Core.notifications API](https://apis.io/apis/aerones/aerones-core-notifications-api/) — The core.notifications API from Aerones — 6 operation(s) for core.notifications.
- [Aerones Core.pipedrive Deals API](https://apis.io/apis/aerones/aerones-core-pipedrive-deals-api/) — The core.pipedrive-deals API from Aerones — 1 operation(s) for core.pipedrive-deals.
- [Aerones Core.planned Resource Set Items.commitments API](https://apis.io/apis/aerones/aerones-core-planned-resource-set-items-commitments-api/) — The core.planned-resource-set-items.commitments API from Aerones — 2 operation(s) for core.planned-resource-set-items.commitments.
- [Aerones Core.planned Resource Sets.items API](https://apis.io/apis/aerones/aerones-core-planned-resource-sets-items-api/) — The core.planned-resource-sets.items API from Aerones — 2 operation(s) for core.planned-resource-sets.items.
- [Aerones Core.positions API](https://apis.io/apis/aerones/aerones-core-positions-api/) — The core.positions API from Aerones — 2 operation(s) for core.positions.
- [Aerones Core.pricing Units API](https://apis.io/apis/aerones/aerones-core-pricing-units-api/) — The core.pricing-units API from Aerones — 1 operation(s) for core.pricing-units.
- [Aerones Core.project Question Configs API](https://apis.io/apis/aerones/aerones-core-project-question-configs-api/) — The core.project-question-configs API from Aerones — 1 operation(s) for core.project-question-configs.
- [Aerones Core.project Scope Change Requests API](https://apis.io/apis/aerones/aerones-core-project-scope-change-requests-api/) — The core.project-scope-change-requests API from Aerones — 5 operation(s) for core.project-scope-change-requests.
- [Aerones Core.project Status API](https://apis.io/apis/aerones/aerones-core-project-status-api/) — The core.project-status API from Aerones — 1 operation(s) for core.project-status.
- [Aerones Core.projects API](https://apis.io/apis/aerones/aerones-core-projects-api/) — The core.projects API from Aerones — 11 operation(s) for core.projects.
- [Aerones Core.projects.billings API](https://apis.io/apis/aerones/aerones-core-projects-billings-api/) — The core.projects.billings API from Aerones — 2 operation(s) for core.projects.billings.
- [Aerones Core.projects.bto API](https://apis.io/apis/aerones/aerones-core-projects-bto-api/) — The core.projects.bto API from Aerones — 5 operation(s) for core.projects.bto.
- [Aerones Core.projects.communication API](https://apis.io/apis/aerones/aerones-core-projects-communication-api/) — The core.projects.communication API from Aerones — 5 operation(s) for core.projects.communication.
- [Aerones Core.projects.contacts API](https://apis.io/apis/aerones/aerones-core-projects-contacts-api/) — The core.projects.contacts API from Aerones — 2 operation(s) for core.projects.contacts.
- [Aerones Core.projects.locations API](https://apis.io/apis/aerones/aerones-core-projects-locations-api/) — The core.projects.locations API from Aerones — 6 operation(s) for core.projects.locations.
- [Aerones Core.projects.offers API](https://apis.io/apis/aerones/aerones-core-projects-offers-api/) — The core.projects.offers API from Aerones — 10 operation(s) for core.projects.offers.
- [Aerones Core.projects.offers.items API](https://apis.io/apis/aerones/aerones-core-projects-offers-items-api/) — The core.projects.offers.items API from Aerones — 3 operation(s) for core.projects.offers.items.
- [Aerones Core.projects.planned Resource Sets API](https://apis.io/apis/aerones/aerones-core-projects-planned-resource-sets-api/) — The core.projects.planned-resource-sets API from Aerones — 2 operation(s) for core.projects.planned-resource-sets.
- [Aerones Core.projects.pre Job Answers API](https://apis.io/apis/aerones/aerones-core-projects-pre-job-answers-api/) — The core.projects.pre-job-answers API from Aerones — 3 operation(s) for core.projects.pre-job-answers.
- [Aerones Core.projects.pre Job Sites API](https://apis.io/apis/aerones/aerones-core-projects-pre-job-sites-api/) — The core.projects.pre-job-sites API from Aerones — 1 operation(s) for core.projects.pre-job-sites.
- [Aerones Core.projects.readiness API](https://apis.io/apis/aerones/aerones-core-projects-readiness-api/) — The core.projects.readiness API from Aerones — 1 operation(s) for core.projects.readiness.
- [Aerones Core.projects.report Types API](https://apis.io/apis/aerones/aerones-core-projects-report-types-api/) — The core.projects.report-types API from Aerones — 2 operation(s) for core.projects.report-types.
- [Aerones Core.projects.resource Sets API](https://apis.io/apis/aerones/aerones-core-projects-resource-sets-api/) — The core.projects.resource-sets API from Aerones — 4 operation(s) for core.projects.resource-sets.
- [Aerones Core.projects.rfi Billing API](https://apis.io/apis/aerones/aerones-core-projects-rfi-billing-api/) — The core.projects.rfi-billing API from Aerones — 1 operation(s) for core.projects.rfi-billing.
- [Aerones Core.projects.scope Items API](https://apis.io/apis/aerones/aerones-core-projects-scope-items-api/) — The core.projects.scope-items API from Aerones — 3 operation(s) for core.projects.scope-items.
- [Aerones Core.purchase Orders API](https://apis.io/apis/aerones/aerones-core-purchase-orders-api/) — The core.purchase-orders API from Aerones — 2 operation(s) for core.purchase-orders.
- [Aerones Core.purchase Orders.projects API](https://apis.io/apis/aerones/aerones-core-purchase-orders-projects-api/) — The core.purchase-orders.projects API from Aerones — 2 operation(s) for core.purchase-orders.projects.
- [Aerones Core.purchase Orders.versions API](https://apis.io/apis/aerones/aerones-core-purchase-orders-versions-api/) — The core.purchase-orders.versions API from Aerones — 3 operation(s) for core.purchase-orders.versions.
- [Aerones Core.regions API](https://apis.io/apis/aerones/aerones-core-regions-api/) — The core.regions API from Aerones — 1 operation(s) for core.regions.
- [Aerones Core.relationship Types API](https://apis.io/apis/aerones/aerones-core-relationship-types-api/) — The core.relationship-types API from Aerones — 1 operation(s) for core.relationship-types.
- [Aerones Core.report Types API](https://apis.io/apis/aerones/aerones-core-report-types-api/) — The core.report-types API from Aerones — 1 operation(s) for core.report-types.
- [Aerones Core.resource Sets API](https://apis.io/apis/aerones/aerones-core-resource-sets-api/) — The core.resource-sets API from Aerones — 2 operation(s) for core.resource-sets.
- [Aerones Core.resources API](https://apis.io/apis/aerones/aerones-core-resources-api/) — The core.resources API from Aerones — 3 operation(s) for core.resources.
- [Aerones Core.resources.certificates API](https://apis.io/apis/aerones/aerones-core-resources-certificates-api/) — The core.resources.certificates API from Aerones — 2 operation(s) for core.resources.certificates.
- [Aerones Core.resources.service Positions API](https://apis.io/apis/aerones/aerones-core-resources-service-positions-api/) — The core.resources.service-positions API from Aerones — 2 operation(s) for core.resources.service-positions.
- [Aerones Core.robot Sets API](https://apis.io/apis/aerones/aerones-core-robot-sets-api/) — The core.robot-sets API from Aerones — 3 operation(s) for core.robot-sets.
- [Aerones Core.robot Sets.services API](https://apis.io/apis/aerones/aerones-core-robot-sets-services-api/) — The core.robot-sets.services API from Aerones — 1 operation(s) for core.robot-sets.services.
- [Aerones Core.service Categories API](https://apis.io/apis/aerones/aerones-core-service-categories-api/) — The core.service-categories API from Aerones — 1 operation(s) for core.service-categories.
- [Aerones Core.service Families API](https://apis.io/apis/aerones/aerones-core-service-families-api/) — The core.service-families API from Aerones — 1 operation(s) for core.service-families.
- [Aerones Core.service Groups API](https://apis.io/apis/aerones/aerones-core-service-groups-api/) — The core.service-groups API from Aerones — 1 operation(s) for core.service-groups.
- [Aerones Core.service Order Lines.lps Results API](https://apis.io/apis/aerones/aerones-core-service-order-lines-lps-results-api/) — The core.service-order-lines.lps-results API from Aerones — 1 operation(s) for core.service-order-lines.lps-results.
- [Aerones Core.service Standard Items API](https://apis.io/apis/aerones/aerones-core-service-standard-items-api/) — The core.service-standard-items API from Aerones — 2 operation(s) for core.service-standard-items.
- [Aerones Core.services API](https://apis.io/apis/aerones/aerones-core-services-api/) — The core.services API from Aerones — 2 operation(s) for core.services.
- [Aerones Core.services.pricing Units API](https://apis.io/apis/aerones/aerones-core-services-pricing-units-api/) — The core.services.pricing-units API from Aerones — 1 operation(s) for core.services.pricing-units.
- [Aerones Core.services.related Services API](https://apis.io/apis/aerones/aerones-core-services-related-services-api/) — The core.services.related-services API from Aerones — 1 operation(s) for core.services.related-services.
- [Aerones Core.standards API](https://apis.io/apis/aerones/aerones-core-standards-api/) — The core.standards API from Aerones — 1 operation(s) for core.standards.
- [Aerones Core.timezones API](https://apis.io/apis/aerones/aerones-core-timezones-api/) — The core.timezones API from Aerones — 1 operation(s) for core.timezones.
- [Aerones Core.turbine Components API](https://apis.io/apis/aerones/aerones-core-turbine-components-api/) — The core.turbine-components API from Aerones — 5 operation(s) for core.turbine-components.
- [Aerones Core.turbine Components.receptors API](https://apis.io/apis/aerones/aerones-core-turbine-components-receptors-api/) — The core.turbine-components.receptors API from Aerones — 1 operation(s) for core.turbine-components.receptors.
- [Aerones Core.turbine Models API](https://apis.io/apis/aerones/aerones-core-turbine-models-api/) — The core.turbine-models API from Aerones — 2 operation(s) for core.turbine-models.
- [Aerones Core.turbine Models.receptor Presets API](https://apis.io/apis/aerones/aerones-core-turbine-models-receptor-presets-api/) — The core.turbine-models.receptor-presets API from Aerones — 3 operation(s) for core.turbine-models.receptor-presets.
- [Aerones Core.turbines API](https://apis.io/apis/aerones/aerones-core-turbines-api/) — The core.turbines API from Aerones — 4 operation(s) for core.turbines.
- [Aerones Core.turbines.receptors API](https://apis.io/apis/aerones/aerones-core-turbines-receptors-api/) — The core.turbines.receptors API from Aerones — 2 operation(s) for core.turbines.receptors.
- [Aerones Core.users API](https://apis.io/apis/aerones/aerones-core-users-api/) — The core.users API from Aerones — 4 operation(s) for core.users.
- [Aerones Core.vendors API](https://apis.io/apis/aerones/aerones-core-vendors-api/) — The core.vendors API from Aerones — 2 operation(s) for core.vendors.
- [Aerones Customer Portal API](https://apis.io/apis/aerones/aerones-customer-portal-api/) — The customer-portal API from Aerones — 2 operation(s) for customer-portal.
- [Aerones Data Tracking API](https://apis.io/apis/aerones/aerones-data-tracking-api/) — The data-tracking API from Aerones — 3 operation(s) for data-tracking.
- [Aerones Deviations API](https://apis.io/apis/aerones/aerones-deviations-api/) — The deviations API from Aerones — 6 operation(s) for deviations.
- [Aerones Dispatch.board Annotations API](https://apis.io/apis/aerones/aerones-dispatch-board-annotations-api/) — The dispatch.board-annotations API from Aerones — 8 operation(s) for dispatch.board-annotations.
- [Aerones Dispatch.board API](https://apis.io/apis/aerones/aerones-dispatch-board-api/) — The dispatch.board API from Aerones — 14 operation(s) for dispatch.board.
- [Aerones Dispatch.board Workorders API](https://apis.io/apis/aerones/aerones-dispatch-board-workorders-api/) — The dispatch.board-workorders API from Aerones — 18 operation(s) for dispatch.board-workorders.
- [Aerones Dispatch.scope Commitments API](https://apis.io/apis/aerones/aerones-dispatch-scope-commitments-api/) — The dispatch.scope-commitments API from Aerones — 10 operation(s) for dispatch.scope-commitments.
- [Aerones Dispatch.services API](https://apis.io/apis/aerones/aerones-dispatch-services-api/) — The dispatch.services API from Aerones — 15 operation(s) for dispatch.services.
- [Aerones Dispatch.workorder Activity Metadata API](https://apis.io/apis/aerones/aerones-dispatch-workorder-activity-metadata-api/) — The dispatch.workorder-activity-metadata API from Aerones — 2 operation(s) for dispatch.workorder-activity-metadata.
- [Aerones Dispatch.workorders API](https://apis.io/apis/aerones/aerones-dispatch-workorders-api/) — The dispatch.workorders API from Aerones — 16 operation(s) for dispatch.workorders.
- [Aerones Docs API](https://apis.io/apis/aerones/aerones-docs-api/) — The docs API from Aerones — 1 operation(s) for docs.
- [Aerones Email API](https://apis.io/apis/aerones/aerones-email-api/) — The email API from Aerones — 4 operation(s) for email.
- [Aerones Files API](https://apis.io/apis/aerones/aerones-files-api/) — The files API from Aerones — 4 operation(s) for files.
- [Aerones Maintainx.assets API](https://apis.io/apis/aerones/aerones-maintainx-assets-api/) — The maintainx.assets API from Aerones — 1 operation(s) for maintainx.assets.
- [Aerones Misc API](https://apis.io/apis/aerones/aerones-misc-api/) — The misc API from Aerones — 10 operation(s) for misc.
- [Aerones Netsuite API](https://apis.io/apis/aerones/aerones-netsuite-api/) — The netsuite API from Aerones — 6 operation(s) for netsuite.
- [Aerones Notifications.events API](https://apis.io/apis/aerones/aerones-notifications-events-api/) — The notifications.events API from Aerones — 1 operation(s) for notifications.events.
- [Aerones Payroll API](https://apis.io/apis/aerones/aerones-payroll-api/) — The payroll API from Aerones — 3 operation(s) for payroll.
- [Aerones Planning API](https://apis.io/apis/aerones/aerones-planning-api/) — The planning API from Aerones — 2 operation(s) for planning.
- [Aerones Planning.campaigns API](https://apis.io/apis/aerones/aerones-planning-campaigns-api/) — The planning.campaigns API from Aerones — 2 operation(s) for planning.campaigns.
- [Aerones Planning.customer Vendors API](https://apis.io/apis/aerones/aerones-planning-customer-vendors-api/) — The planning.customer-vendors API from Aerones — 2 operation(s) for planning.customer-vendors.
- [Aerones Planning.projects API](https://apis.io/apis/aerones/aerones-planning-projects-api/) — The planning.projects API from Aerones — 2 operation(s) for planning.projects.
- [Aerones Planning.service Orders API](https://apis.io/apis/aerones/aerones-planning-service-orders-api/) — The planning.service-orders API from Aerones — 2 operation(s) for planning.service-orders.
- [Aerones Planning.services API](https://apis.io/apis/aerones/aerones-planning-services-api/) — The planning.services API from Aerones — 2 operation(s) for planning.services.
- [Aerones Planning.statuses API](https://apis.io/apis/aerones/aerones-planning-statuses-api/) — The planning.statuses API from Aerones — 1 operation(s) for planning.statuses.
- [Aerones Planning.work Order Types API](https://apis.io/apis/aerones/aerones-planning-work-order-types-api/) — The planning.work-order-types API from Aerones — 2 operation(s) for planning.work-order-types.
- [Aerones Planning.work Orders API](https://apis.io/apis/aerones/aerones-planning-work-orders-api/) — The planning.work-orders API from Aerones — 2 operation(s) for planning.work-orders.
- [Aerones Platform API](https://apis.io/apis/aerones/aerones-platform-api/) — The platform API from Aerones — 2 operation(s) for platform.
- [Aerones Projects.accounting API](https://apis.io/apis/aerones/aerones-projects-accounting-api/) — The projects.accounting API from Aerones — 37 operation(s) for projects.accounting.
- [Aerones Projects.bto API](https://apis.io/apis/aerones/aerones-projects-bto-api/) — The projects.bto API from Aerones — 1 operation(s) for projects.bto.
- [Aerones Projects.core API](https://apis.io/apis/aerones/aerones-projects-core-api/) — The projects.core API from Aerones — 8 operation(s) for projects.core.
- [Aerones Projects.offer API](https://apis.io/apis/aerones/aerones-projects-offer-api/) — The projects.offer API from Aerones — 5 operation(s) for projects.offer.
- [Aerones Projects.offer.changelog API](https://apis.io/apis/aerones/aerones-projects-offer-changelog-api/) — The projects.offer.changelog API from Aerones — 6 operation(s) for projects.offer.changelog.
- [Aerones Projects.overview API](https://apis.io/apis/aerones/aerones-projects-overview-api/) — The projects.overview API from Aerones — 2 operation(s) for projects.overview.
- [Aerones Projects.platform API](https://apis.io/apis/aerones/aerones-projects-platform-api/) — The projects.platform API from Aerones — 1 operation(s) for projects.platform.
- [Aerones Projects.pre Job API](https://apis.io/apis/aerones/aerones-projects-pre-job-api/) — The projects.pre-job API from Aerones — 1 operation(s) for projects.pre-job.
- [Aerones Projects.pre Job.assets Services API](https://apis.io/apis/aerones/aerones-projects-pre-job-assets-services-api/) — The projects.pre-job.assets-services API from Aerones — 1 operation(s) for projects.pre-job.assets-services.
- [Aerones Projects.pre Job.assets Services.table API](https://apis.io/apis/aerones/aerones-projects-pre-job-assets-services-table-api/) — The projects.pre-job.assets-services.table API from Aerones — 4 operation(s) for projects.pre-job.assets-services.table.
- [Aerones Projects.rams API](https://apis.io/apis/aerones/aerones-projects-rams-api/) — The projects.rams API from Aerones — 20 operation(s) for projects.rams.
- [Aerones Projects.rams Templates API](https://apis.io/apis/aerones/aerones-projects-rams-templates-api/) — The projects.rams-templates API from Aerones — 6 operation(s) for projects.rams-templates.
- [Aerones Projects.reporting Requirements API](https://apis.io/apis/aerones/aerones-projects-reporting-requirements-api/) — The projects.reporting-requirements API from Aerones — 4 operation(s) for projects.reporting-requirements.
- [Aerones Projects.rfi API](https://apis.io/apis/aerones/aerones-projects-rfi-api/) — The projects.rfi API from Aerones — 7 operation(s) for projects.rfi.
- [Aerones Projects.robot Sets And Teams API](https://apis.io/apis/aerones/aerones-projects-robot-sets-and-teams-api/) — The projects.robot-sets-and-teams API from Aerones — 4 operation(s) for projects.robot-sets-and-teams.
- [Aerones Projects.service Orders API](https://apis.io/apis/aerones/aerones-projects-service-orders-api/) — The projects.service-orders API from Aerones — 20 operation(s) for projects.service-orders.
- [Aerones Projects.set Demobs API](https://apis.io/apis/aerones/aerones-projects-set-demobs-api/) — The projects.set-demobs API from Aerones — 8 operation(s) for projects.set-demobs.
- [Aerones Projects.set Requests API](https://apis.io/apis/aerones/aerones-projects-set-requests-api/) — The projects.set-requests API from Aerones — 21 operation(s) for projects.set-requests.
- [Aerones Projects.team Requests API](https://apis.io/apis/aerones/aerones-projects-team-requests-api/) — The projects.team-requests API from Aerones — 21 operation(s) for projects.team-requests.
- [Aerones Projects.upcoming Rotations API](https://apis.io/apis/aerones/aerones-projects-upcoming-rotations-api/) — The projects.upcoming-rotations API from Aerones — 1 operation(s) for projects.upcoming-rotations.
- [Aerones Projects.weather API](https://apis.io/apis/aerones/aerones-projects-weather-api/) — The projects.weather API from Aerones — 4 operation(s) for projects.weather.
- [Aerones Projects.workorders API](https://apis.io/apis/aerones/aerones-projects-workorders-api/) — The projects.workorders API from Aerones — 2 operation(s) for projects.workorders.
- [Aerones Readiness API](https://apis.io/apis/aerones/aerones-readiness-api/) — The readiness API from Aerones — 1 operation(s) for readiness.
- [Aerones Reporting Requirements.cru API](https://apis.io/apis/aerones/aerones-reporting-requirements-cru-api/) — The reporting-requirements.cru API from Aerones — 9 operation(s) for reporting-requirements.cru.
- [Aerones Reports API](https://apis.io/apis/aerones/aerones-reports-api/) — The reports API from Aerones — 7 operation(s) for reports.
- [Aerones Resource Mobilization.obd Gps Devices API](https://apis.io/apis/aerones/aerones-resource-mobilization-obd-gps-devices-api/) — The resource-mobilization.obd-gps-devices API from Aerones — 6 operation(s) for resource-mobilization.obd-gps-devices.
- [Aerones Resource Mobilization.vehicle Fleet Assignments API](https://apis.io/apis/aerones/aerones-resource-mobilization-vehicle-fleet-assignments-api/) — The resource-mobilization.vehicle-fleet-assignments API from Aerones — 11 operation(s) for resource-mobilization.vehicle-fleet-assignments.
- [Aerones Resource Mobilization.vehicle Fleet Invoices API](https://apis.io/apis/aerones/aerones-resource-mobilization-vehicle-fleet-invoices-api/) — The resource-mobilization.vehicle-fleet-invoices API from Aerones — 6 operation(s) for resource-mobilization.vehicle-fleet-invoices.
- [Aerones Resource Mobilization.vehicle Fleet Locations API](https://apis.io/apis/aerones/aerones-resource-mobilization-vehicle-fleet-locations-api/) — The resource-mobilization.vehicle-fleet-locations API from Aerones — 2 operation(s) for resource-mobilization.vehicle-fleet-locations.
- [Aerones Resource Mobilization.vehicles API](https://apis.io/apis/aerones/aerones-resource-mobilization-vehicles-api/) — The resource-mobilization.vehicles API from Aerones — 7 operation(s) for resource-mobilization.vehicles.
- [Aerones Services API](https://apis.io/apis/aerones/aerones-services-api/) — The services API from Aerones — 3 operation(s) for services.
- [Aerones Talentlms.users API](https://apis.io/apis/aerones/aerones-talentlms-users-api/) — The talentlms.users API from Aerones — 1 operation(s) for talentlms.users.
- [Aerones Technician.projects API](https://apis.io/apis/aerones/aerones-technician-projects-api/) — The technician.projects API from Aerones — 3 operation(s) for technician.projects.
- [Aerones Technician.reports API](https://apis.io/apis/aerones/aerones-technician-reports-api/) — The technician.reports API from Aerones — 11 operation(s) for technician.reports.
- [Aerones Technician.service Results API](https://apis.io/apis/aerones/aerones-technician-service-results-api/) — The technician.service_results API from Aerones — 8 operation(s) for technician.service_results.
- [Aerones Technician.workorders API](https://apis.io/apis/aerones/aerones-technician-workorders-api/) — The technician.workorders API from Aerones — 6 operation(s) for technician.workorders.
- [Aerones Turbines API](https://apis.io/apis/aerones/aerones-turbines-api/) — The turbines API from Aerones — 7 operation(s) for turbines.
- [Aerones Users API](https://apis.io/apis/aerones/aerones-users-api/) — The users API from Aerones — 2 operation(s) for users.
- [Aerones Utilities API](https://apis.io/apis/aerones/aerones-utilities-api/) — The utilities API from Aerones — 1 operation(s) for utilities.
- [Aerones Vis.ai Anomalies API](https://apis.io/apis/aerones/aerones-vis-ai-anomalies-api/) — The vis.ai-anomalies API from Aerones — 5 operation(s) for vis.ai-anomalies.
- [Aerones Vis.external Photos API](https://apis.io/apis/aerones/aerones-vis-external-photos-api/) — The vis.external-photos API from Aerones — 1 operation(s) for vis.external-photos.
- [Aerones Vis.inspections API](https://apis.io/apis/aerones/aerones-vis-inspections-api/) — The vis.inspections API from Aerones — 4 operation(s) for vis.inspections.
- [Aerones Vis.pointclouds API](https://apis.io/apis/aerones/aerones-vis-pointclouds-api/) — The vis.pointclouds API from Aerones — 1 operation(s) for vis.pointclouds.
- [Aerones Vis.root Photos API](https://apis.io/apis/aerones/aerones-vis-root-photos-api/) — The vis.root-photos API from Aerones — 1 operation(s) for vis.root-photos.
- [Aerones Vis.rosbags API](https://apis.io/apis/aerones/aerones-vis-rosbags-api/) — The vis.rosbags API from Aerones — 2 operation(s) for vis.rosbags.
- [Aerones Vis.video Files API](https://apis.io/apis/aerones/aerones-vis-video-files-api/) — The vis.video-files API from Aerones — 3 operation(s) for vis.video-files.
- [Aerones Webhooks API](https://apis.io/apis/aerones/aerones-webhooks-api/) — The webhooks API from Aerones — 5 operation(s) for webhooks.
- [Aerones Webhooks.travel API](https://apis.io/apis/aerones/aerones-webhooks-travel-api/) — The webhooks.travel API from Aerones — 1 operation(s) for webhooks.travel.
- [Aerones Webhooks.wms API](https://apis.io/apis/aerones/aerones-webhooks-wms-api/) — The webhooks.wms API from Aerones — 1 operation(s) for webhooks.wms.
- [Aerones Wms API](https://apis.io/apis/aerones/aerones-wms-api/) — The wms API from Aerones — 6 operation(s) for wms.
- [Aerones Work Management.activities API](https://apis.io/apis/aerones/aerones-work-management-activities-api/) — The work-management.activities API from Aerones — 7 operation(s) for work-management.activities.
- [Aerones Work Management.activity Templates API](https://apis.io/apis/aerones/aerones-work-management-activity-templates-api/) — The work-management.activity-templates API from Aerones — 2 operation(s) for work-management.activity-templates.
- [Aerones Work Management.anomaly Work Orders API](https://apis.io/apis/aerones/aerones-work-management-anomaly-work-orders-api/) — The work-management.anomaly-work-orders API from Aerones — 2 operation(s) for work-management.anomaly-work-orders.
- [Aerones Work Management.campaigns API](https://apis.io/apis/aerones/aerones-work-management-campaigns-api/) — The work-management.campaigns API from Aerones — 7 operation(s) for work-management.campaigns.
- [Aerones Work Management.client Work Orders API](https://apis.io/apis/aerones/aerones-work-management-client-work-orders-api/) — The work-management.client-work-orders API from Aerones — 8 operation(s) for work-management.client-work-orders.
- [Aerones Work Management.statuses API](https://apis.io/apis/aerones/aerones-work-management-statuses-api/) — The work-management.statuses API from Aerones — 1 operation(s) for work-management.statuses.
- [Aerones Work Management.task Types API](https://apis.io/apis/aerones/aerones-work-management-task-types-api/) — The work-management.task-types API from Aerones — 2 operation(s) for work-management.task-types.
- [Aerones Work Management.vendors API](https://apis.io/apis/aerones/aerones-work-management-vendors-api/) — The work-management.vendors API from Aerones — 2 operation(s) for work-management.vendors.
- [Aerones Work Management.work Packages API](https://apis.io/apis/aerones/aerones-work-management-work-packages-api/) — The work-management.work-packages API from Aerones — 8 operation(s) for work-management.work-packages.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Aerones Event Surface](https://apis.io/asyncapis/aerones/aerones-event-surface/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [aerones-operations-hub](https://apis.io/servers/aerones/aerones-operations-hub/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Aerones Operations Hub Overlay](https://apis.io/overlays/aerones/aerones-operations-hub-overlay/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Aerones Authentication](https://apis.io/security/aerones/aerones-authentication/)
- [Aerones Domain Security](https://apis.io/security/aerones/aerones-domain-security/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Aerones Scopes](https://apis.io/scopes/aerones/aerones-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Aerones Plans Pricing](https://apis.io/plans/aerones/aerones-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Aerones Rate Limits](https://apis.io/rate-limits/aerones/aerones-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://aerones.com/)
- [API reference](https://operations.aerones.com/api/docs)
- [Support](https://aerones.com/our-contacts/)
- [Blog](https://aerones.com/news/)
- [Compliance](https://aerones.com/certification/)
- [Terms of service](https://aerones.com/terms-and-conditions/)
- [Privacy policy](https://aerones.com/privacy-policy/)

## API Evangelist rating

**Kin Score 47.0** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 57.9 |
| Contract governance | 18.2 |
| Operational transparency | 0.0 |
| Developer ergonomics | 20.8 |
| Access clarity | 28.9 |

**Agent readiness 44.4** — agent-ready (gated down from agent-native)

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | verified |
| MCP Server | — |
| Auth Clarity | served (partial credit) |
| Idempotency | derived (partial credit) |
| Error Semantics | verified |
| OpenAPI Examples | partial |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | derived (partial credit) |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | served (partial credit) |
| Protected Resource Metadata | — |
| Dynamic Client Registration | yes |
| Agentic Commerce | — |
| Pagination Ratio | partial |
| Operation Distinctiveness | mostly |

**Regulatory alignment 38.5** — Energy & Utilities

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/aerones/](https://apis.io/providers/aerones/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Aerones: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/aerones/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
