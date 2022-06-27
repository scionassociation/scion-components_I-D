---
title: "SCION Components Analysis"
abbrev: "SCION COMP I-D"
category: info
submissiontype: IRTF

docname: draft-rustignoli-panrg-scion-components-latest
v: 3
area: "IRTF"
workgroup: "Path Aware Networking RG"
keyword: Internet-Draft
venue:
  group: "Path Aware Networking RG"
  type: "Research Group"
  mail: "panrg@irtf.org"
  arch: "https://www.ietf.org/mail-archive/web/panrg/"
  github: "scionassociation/scion-components_I-D"
  latest: "https://scionassociation.github.io/scion-components_I-D/draft-rustignoli-panrg-scion-components.html"

author:
 -   ins: N. Rustignoli
     name: Nicola Rustignoli
     org: ETH Zuerich
     email: nicola.rustignoli@inf.ethz.ch

 -   ins: C. de Kater
     name: Corine de Kater
     org: ETH Zuerich
     email: corine.dekatermuehlhaeuser@inf.ethz.ch

 -   ins: A. Perrig
     name: Adrian Perrig
     org: ETH Zuerich
     email: adrian.perrig@inf.ethz.ch

normative:


informative:
  RFC4264:
  RFC4033:
  RFC5218:
  RFC6480:
  RFC6830:
  RFC8205:
  RFC8446:
  RFC9049:
  RFC9217:
  RFC8170:
  RFC4443:
  RFC0791:
  SCHUCHARD2011: DOI.10.1145/1866307.1866411
  LABOVITZ2000: DOI.10.1145/347059.347428
  GRIFFIN1999: DOI.10.1145/316194.316231
  SAHOO2009: DOI.10.1016/j.comcom.2009.03.009
  LYCHEV2013: DOI.10.1145/2534169.2486010
  LI2014: DOI.10.14722/sent.2014.23001
  COOPER2013: DOI.10.1145/2535771.2535787
  ROTHENBERGER2017: DOI.10.1145/3065913.3065922
  MORILLO2021: DOI.10.14722/ndss.2021.24438
  KLENZE2021: DOI.10.1109/CSF51468.2021.00018
  DERUITER2021: DOI.10.1145/3485983.3494839
  ANDERSEN2001: DOI.10.1145/502034.502048
  KATZ2012: DOI.10.1145/2377677.2377756
  KUSHMAN2007: DOI.10.1145/1232919.1232927
  PERRIG2017:
    title: "SCION: A Secure Internet Architecture"
    date: 2017
    target: https://doi.org/10.1007/978-3-319-67080-5
    seriesinfo:
      ISBN: 978-3-319-67079-9
    author:
      -
        ins: A. Perrig
        name: Adrian Perrig
        org: ETH Zuerich
      -
        ins: P. Szalachowski
        name: Pawel Szalachowski
        org: ETH Zuerich
      -
        ins: R. Reischuk
        name: Raphael Reischuk
        org: ETH Zuerich
      -
        ins: L. Chuat
        name: Laurent Chuat
        org: ETH Zuerich
  DEKATER2022:
    title: SCION Overview
    date: 2022
    target: https://datatracker.ietf.org/doc/draft-dekater-panrg-scion-overview/
    author:
      -
        ins: C. de Kater
        name: Corine de Kater
        org: ETH Zuerich
      -
        ins: A. Farrel
        name: Nicola Rustignoli
        org: ETH Zuerich
      -
        ins: A. Perrig
        name: Adrian Perrig
        org: ETH Zuerich
  HITZ2021:
    title: Demonstrating the reliability and resilience of Secure Swiss Finance Network
    date: 2021
    target: https://perma.cc/4H3Q-WZNG
    author:
      ins: S. Hitz
      name: Samuel Hitz
      org: Anapaya Systems
  LEGNER2020:
     title: "EPIC: Every Packet Is Checked in the Data Plane of a Path-Aware Internet"
     date: 2020
     target: https://www.usenix.org/conference/usenixsecurity20/presentation/legner
     author:
       -
         ins: M. Legner
         name: Adrian Perrig
         org: ETH Zuerich
       -
         ins: T. Klenze
         name: Tobias Klenze
         org: ETH Zuerich
       -
         ins: M. Wyss
         name: Marc Wyss
         org: ETH Zuerich
       -
         ins: C. Sprenger
         name: Christoph Sprenger
         org: ETH Zuerich
       -
         ins: A. Perrig
         name: Adrian Perrig
         org: ETH Zuerich
  CHUAT22:
    title: "The Complete Guide to SCION"
    date: 2022
    target: https://doi.org/10.1007/978-3-031-05288-0
    seriesinfo:
      ISBN: 978-3-031-05287-3
    author:
      -
        ins: L. Chuat
        name: Laurent Chuat
        org: ETH Zuerich
      -
        ins: M. Legner
        name: Markus Legner
        org: ETH Zuerich
      -
        ins: D. Basin
        name: David Basin
        org: ETH Zuerich
      -
        ins: D. Hausheer
        name: David Hausheer
        org: Otto von Guericke University Magdeburg
      -
        ins: S. Hitz
        name: Samuel Hitz
        org: Anapaya Systems
      -
        ins: P. Mueller
        name: Peter Mueller
        org: ETH Zuerich
      -
        ins: A. Perrig
        name: Adrian Perrig
        org: ETH Zuerich
  PANRG-INTERIM-Min:
    title: Path Aware Networking Research Group - Interim  106 Minutes
    date: June 2022
    target: https://datatracker.ietf.org/meeting/interim-2022-panrg-01/materials/minutes-interim-2022-panrg-01-202206011700-00


--- abstract

SCION is a future Internet architecture that focuses on security and availability. Its fundamental functions are carried out by a number of components.

This document illustrates the dependencies between its core components, extensions. We also discuss the relationship between SCION and existing protocols, with focus on illustrating which existing protocols are reused/extended. We also describe the motivations behind cases where a greenfield approach is needed. We also briefly touch on the maturity level of components.

--- middle

# Introduction

While SCION  was initially developed in academia, the architecture  has now "slipped out of the lab" and counts its early productive deployments (including the Swiss inter-banking network SSFN).
The architecture consists of a system of related components, some of which are  essential to set up end to end SCION connectivity, while others are add-ons aiming at providing additional functionality, security, or backwards compatibility. Discussions at {{PANRG-INTERIM-Min}} showed the need to describe the relationships between SCION's core components.
In this document we therefore focus on each component, describing its functionality, dependencies and relationships to existing protocols. The goal is not to describe each component specification, rather to provide a basis for discussions about the engineering decisions that made SCION what it is.
Before reading this document, please refer to {{DEKATER2022}} for a generic overview of SCION and its components, the problems it solves, and existing deployments. For an in-depth description of SCION, please refer to {{CHUAT22}}.
TODO: IMHO while in the other draft we focused on describing services and how each component works, now we need to focus on describing why each component works the way it does...

## Conventions and Definitions

{::boilerplate bcp14-tagged}

# Minimal stack - core components
In order to establish end to end connectivity, SCION relies on three main components.
SCION's data plane carries out secure path-aware forwarding. Its control plane takes case of routing. SCION relies on the Control Plane PKI to handle cryptographic material.

The control plane is responsible for discovering and disseminating routing information. Route discovery is performed by each autonomous system (AS) thanks to an authenticated path-exploration mechanism called beaconing.
SCION end hosts query their respective AS control plane and obtain authenticated and authorized network paths, in the form of path segments.
End hosts select one or more of the end to end network paths, based on the application requirements (i.e.,  latency). End hosts then craft SCION packets containing the end-to end path to the destination.
The data plane is responsible for forwarding SCION packets while authenticating them at each hop and.

Both the control and data plane rely on the control-plane PKI for authentication and authorization.
SCION's authentication mechanisms aim at protecting the whole end to end path at each hop. SCION Autonomous systems are organised in Isolation Domains (ISDs), that independently define their own roots of trust.
ISD members share an uniform trust environment (i.e., a common jurisdiction).
They can transparently define trust relationships between parts of the network by deciding wether to trust other ISDs.
SCION therefore relies on an unique trust model, which is markably different from other PKI. We clarify the motivation behind this in [Authentication](#pki)



All components are deployed in production (i.e. they power the SSFN, there are multiple implementations). They have multiple implementations (including a high performance one).

## Routing - Control Plane
TODO: use content that was discarded in overview draft (SCION vs BGP, SCION vs RPKI) https://github.com/scionassociation/scion-overview_I-D/blob/8259808cbbd41e8c1d8e39eb7ffc63b8d516433c/draft-perrig-scion-overview.md

IP comes with the following drawbacks:

- **Lack of programmable paths**
IP addressing is tightly coupled with routing, therefore packets follow the path established by the routing protocol. End hosts are not able to select paths based on application requirements or path conditions. In addition, it is also not possible to simultaneously use multiple distinct paths towards the same destination.
- **Lack of security and transparency**
IP end hosts are oblivious to the path taken by their packets. This means that end hosts have no visibility nor guarantees on where their traffic is forwarded. This may cause traffic to be redirected through adversary points, breaching the payload's security.
- **Scalability**
The use of forwarding tables in IP routers is time-consuming, expensive, and energy-intensive. Also, the constantly growing size of forwarding tables causes storage problems. Additionally, routers that keep state for network information can suffer from denial-of-service (DoS) attacks exhausting the router’s state {{SCHUCHARD2011}}.

#### BGP

Just as IP, also BGP suffers from a number of shortcomings:

- **Convergence time in case of outages**
The distributed nature of BGP control plane results in convergence times up to ten minutes or more {{LABOVITZ2000}}, resulting in slow failover and intermittent transient connectivity.
- **Lack of fault isolation**
Due to the lack of any routing hierarchy or isolation between different areas, a single faulty BGP speaker can affect routing in the entire world.
- **Poor scalability**
As the number of connected devices grows, so does the number of prefixes, posing additional strain on the protocol. Scalability challenges are particularly evident when considering  BGPSec {{RFC8205}}.
- **Convergence**
BGP convergence can be problematic, too. In certain situations, BGP will never converge to a stable state, or converge only non-deterministically (see {{GRIFFIN1999}} and {{RFC4264}}. Convergence may also take too much time {{SAHOO2009}}.
- **Single path**
BGP only allows the selection of a single path to a destination. But having a multi-path choice can be welcome in several situations, e.g., in the case of a link failure, for load balancing, or when traffic is routed based on different policies.
- **Lack of security**
BGP has no built-in security mechanisms and does not provide any tools for ASes to authenticate the information they receive through BGP update messages. This opens up a multitude of attack opportunities.

- **Problems with BGPsec in partial deployment**
BGPsec only provides full security when all ASes consistently use and enforce it. In case of partial deployment, it has a limited effectiveness. It can even cause instabilities and is prone to downgrade attacks, see {{LYCHEV2013}}.
- **Problems with BGPsec in full deployment**
Also full deployment of BGPsec raises issues, such as the creation of wormholes and forwarding loops by attackers, or the introduction of circular dependencies, see {{LI2014}} and {{COOPER2013}}. RPKI and BGPsec together also cause issues for network sovereignty {{ROTHENBERGER2017}}.
- **Scalability** BGPsec further exacerbates BGP’s scalability issues (i.e., due to the additional overhead, and due to lack of prefix aggregation). Lack of scalable implementations represent still today a large obstacle to adoption.


## Need for Isolation Domains
TODO: their goals are clearly stated in the other draft

## Forwarding - Data plane

###  SCION and Segment Routing

## Authentication -  SCION PKI {#pki}
TODO: why do we need a strong PKI?
* Talk about monopoly vs oligopoly and why this is important (but maybe in the CP part)?
* Why we could not just use RPKI 9that we use for origin validation)
This makes the SCION CP-PKI distinct from other PKIs (i.e. web PKI, RPKI), that either have a single root of trust root (monopoly model), or rely on a plethora of roots of trust (oligopoly model) leading to a trust architecture that supports meaningful trust roots in a global environment with inherently distrustful entities.


### Issues with RPKI and BGPsec

 RPKI and BGPsec try to address Internet's above-mentioned security shortcomings, see also {{RFC6480}} and {{RFC8205}}. However, RPKI and BGPsec introduce additional challenges, as shortly described below.

- **RPKI and Route Origin Authorizations**
Unfortunately, the Route Origin Authorizations (ROAs) provided by RPKI only prevent the simplest form of BGP hijacks.

#### Lack of Authentication

Authenticating digital data is becoming increasingly prevalent, as adversaries exploit the absence of authentication to inject malicious information. Specifically, many network protocols do not use authentication at all, leaving them exposed to multiple attacks:

- Today's Internet lacks a fundamental mechanism to share a secret key between two end hosts for secure end-to-end communication. Existing approaches (i.e., SSH) resort to trust-on-first-use (TOFU) approach, where an host's initial public key is accepted without verification.
- Infrastructures were added over time to provide authentication, such as RPKI/BGPsec, TLS {{RFC8446}}, and DNSSEC {{RFC4033}}. However, they  are all sensitive to the compromise of a single entity.
- The Internet Control Message Protocol (ICMP) lacks an authenticated counterpart, see {{RFC4443}} and {{RFC0791}}. Unauthenticated ICMP messages can potentially be used to affect or even prevent traffic forwarding. TODO: complete


# Additional components
TODO:
- Happy eyeballs (and how we extend things)
- SIAM (& how it piggybacks onto RPKI)
- DrKey & dependencies --> https://datatracker.ietf.org/doc/draft-garciapardo-panrg-drkey/
  - LightningFilter --> https://datatracker.ietf.org/meeting/111/materials/slides-111-panrg-lightning-filter-high-speed-traffic-filtering-based-on-drkey
  - SCMP

# Transition mechanisms
TODO:
* Mention that there are multiple mechanisms, requiring different levels of changes and with different maturity.
* For each nmeachanism, provide a short summary of the approach, what it dies and what protocols it reuses/extends
  * SIG
  * SBAS
  * SIAM

# Dependency analysis

# Motivations for greenfield approaches {{RFC9049}}
TODO: in our overview draft, we said that we would clarify the motivations for developing SCION in another draft. This one could be the one..
*  properties that want to achieve (motivating them with RFC9049). (Maybe we can do this per-component)?
*  why achieving these properties requires a greenfield approach
* why this is the only way to differentiate from the previous failed approaches mentioned in RFC9049.



# Security Considerations

TODO Security


# IANA Considerations

This document has no IANA actions.


--- back

# Acknowledgments
{:numbered="false"}

TODO acknowledge.
