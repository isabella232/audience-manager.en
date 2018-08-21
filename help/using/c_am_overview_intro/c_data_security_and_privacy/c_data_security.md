---
description: Audience Manager takes data security and privacy very seriously. We work to keep our systems secure and protect your valuable data.
seo-description: Audience Manager takes data security and privacy very seriously. We work to keep our systems secure and protect your valuable data.
seo-title: Data Security
solution: Audience Manager
title: Data Security
uuid: 4bf6b559-ea0e-4cc8-9d51-8f6241edcf9e
index: y
internal: n
snippet: y
translate: y
---

# Data Security

Audience Manager security practices include external and internal audits, activity logging, training, and other procedures designed to help protect our systems and your valuable data. We believe a secure product helps build and maintain the trust customers place in us. 

In Audience Manager, we think about security in three main categories: 

|  Security Type  | Provides Support For  |
|---|---|
| **Information security** | Enterprise-level authentication, encryption, and data storage practices  |
| **Data leakage/transparency** | Deep and actionable insight into on-site activities that constitute or contribute to data leakage  |
| **Process/policy enhancements** | Clients, by working with industry best practices for privacy and data security  |

This topic contains the following information: 

* [ Systems, Training, and Access ](../../c_am_overview_intro/c_data_security_and_privacy/c_data_security.md#section_226017634A9945098327561285335D71)
* [ Privacy and Personally Identifiable Information (PII) ](../../c_am_overview_intro/c_data_security_and_privacy/c_data_security.md#section_3F60A967DDD24592B0349831D4E865A3)
* [ Data Partitioning ](../../c_am_overview_intro/c_data_security_and_privacy/c_data_security.md#section_0F061AB523EC420D9F9505E5B97F31C1)
* [ Inbound Server-to-Server (S2S) Transfers ](../../c_am_overview_intro/c_data_security_and_privacy/c_data_security.md#section_1A3DA20297AD4AC08AE8C9D815E22601)
* [ Protecting Data ](../../c_am_overview_intro/c_data_security_and_privacy/c_data_security.md#section_B1F060DCC62A4462A408C76A687BE6BE)

## Systems, Training, and Access {#section_226017634A9945098327561285335D71}

Processes that help keep our system and your data secure. 

**External Security Validation: ** Audience Manager tests security on an annual and quarterly basis. 
* Yearly: Once a year, Audience Manager undergoes a full penetration test conducted by an independent third-party company. The test is designed to identify security vulnerabilities in the application. The tests include scanning for cross-site scripting, SQL injections, form parameter manipulation, and other application-level vulnerabilities.
* Quarterly: Once each quarter, internal teams check for security vulnerabilities. These tests include network scans for open ports and service vulnerabilities.


**Systems Security: ** To help keep data safe and private, Audience Manager: 

* Blocks requests from unauthorized IP addresses.
* Protects data behind firewalls, VPNs, and with Virtual Private Cloud storage.
* Tracks changes in the customer and control-information databases with trigger-based audit logging. These logs track all changes at the database level, including the user ID and IP address from which changes are made.
**Security Assets: ** Audience Manager has a dedicated network operations team that monitors firewalls and intrusion-detection devices. Only key personnel have access to our security technology and data. 

**Security Training: ** Internally, our commitment to security extends to developers who work on our product. Adobe provides formal training to developers on how to build secure applications and services. 

**Secure Access: ** Audience Manager requires strong passwords to log on to the system. See [ password requirements](../../c_reference/c_password_requirements.md#concept_0B501857C23944DCAE4875D3F9455F5F). 

## Privacy and Personally Identifiable Information (PII) {#section_3F60A967DDD24592B0349831D4E865A3}

Processes that help keep personal information safe. For additional privacy information, see the[ Adobe Privacy Center](http://www.adobe.com/privacy/advertising-services.html). **PII Data: ** Audience Manager contractually prohibits customers and data partners from sending PII information into our system. Additionally, the Unique User ID (UUID) does not contain or use PII data as part of the ID-generation algorithm. 

**IP Addresses: ** Audience Manager does collect IP addresses. IP addresses are used in data-processing and log-aggregation processes. They are also required for geographic/location look-ups and targeting. Additionally, all IP addresses within retained log files are obfuscated within 90 days. 

## Data Partitioning {#section_0F061AB523EC420D9F9505E5B97F31C1}

Processes that help protect data owned by individual clients. 

**Trait Data Partitioning: ** Your data (traits, IDs, etc.) is partitioned by client. This helps prevent accidental information exposure between different clients. For example, trait data in cookies is partitioned by customer and stored in a client-specific sub-domain. It cannot be read or used accidentally by another Audience Manager client. Furthermore, trait data stored in the Profile Cache Servers (PCS) is also partitioned by customer. This prevents other clients from accidentally using your data in an event call or other request. 

**Data Partitioning in Reports: ** Client IDs are part of the identifying key in all reporting tables and report queries are filtered by ID. This helps prevent your data from appearing in the reports of another Audience Manager customer. 