---
title: Applicability Statement for the AS112 Project
docname: draft-jabley-dnsop-as112-applicability-00
updates: 7534

submissiontype: IETF
ipr: trust200902
area: Internet
wg: DNSOP Working Group
kw: Internet-Draft
cat: bcp

coding: us-ascii
pi:
  - toc
  - symrefs
  - sortrefs

author:
  -
    ins: J. Abley
    name: Joe Abley
    org: Cloudflare
    city: Amsterdam
    country: NL
    email: jabley@cloudflare.com
  -
    ins: W. Kumari
    name: Warren Kumari
    org: Google

--- abstract

The AS112 Project provides infrastructure that is used as a target for
DNS queries that it is not possible to answer in a useful way, such as
queries that relate to a private network that are sent to a public
server. From time to time IETF protocols specify use of the AS112
Project. This document provides an Applicability Statement for the
AS112 Project that aims to provide guidance for how and when the
AS112 Project should be used.

--- middle

# Introduction

Well, how about this.

# Terminology used in this document

The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT",
"SHOULD", "SHOULD NOT", "RECOMMENDED", "NOT RECOMMENDED", "MAY",
and "OPTIONAL" in this document are to be interpreted as described
in BCP 14 {{!RFC2119}} {{!RFC8174}} when, and only when, they appear
in all capitals, as shown here.

This document makes use of DNS terminology as defined in {{!RFC9499}}.

# Operational Considerations of the AS112 Project

When and how to use the AS112 project in general.

# Use of the AS112 Project in IETF Protocols

## How to ask the IANA to do things

# Security Considerations

Make reference to the existing security guidance.

Provide guidance on when sinking queries with the AS112 project is appropriate, and when it is not. For example, note that causing queries to be redirected to AS112 servers can present privacy risks.

Note that protocols that intend to cause queries to be sent to AS112 servers should do so carefully, mindful that excessive traffic being sent to any destination can have the effect of denying service to both AS112 infrastructure and intermediate networks and systems.

# IANA Considerations

Give IANA directions about how to respond to requests from other documents that relate to AS112.

Note that since there are known cases of protocols that specify that queries for particular names in the ARPA domain be redirected to AS112 infrastructure, the IANA should start the process of becoming equipped to provision DNAME RRSets in the ARPA zone. Perhaps clarify that the provisioning process involves ancilliary systems and processes and is not simply a matter of support for the DNAME resource record type in the servers that serve the ARPA zone.

# Acknowledgements

These people helped.

--- back

# This is an appendix.

