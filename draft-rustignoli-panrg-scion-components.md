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
  RFC7911:
  RFC8205:
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
  KRAHENBUHL2022:
     title: "Deployment and Scalability of an Inter-Domain Multi-Path Routing Infrastructure"
     date: 2022
     target: https://netsec.ethz.ch/publications/papers/2021_conext_deployment.pdf
     author:
       -
         ins: C. Krähenbühl
         name: Cyrill Krähenbühl
         org: ETH Zuerich
       -
         ins: S. Tabaeiaghdaei
         name: Seyedali Tabaeiaghdaei
         org: ETH Zuerich
       -
         ins: C. Glοοr
         name: Christelle Glοοr
         org: ETH Zuerich
       -
         ins: J. Kwon
         name: Jonghoon Kwon
         org: ETH Zuerich
       -
         ins: A. Perrig
         name: Adrian Perrig
         org: ETH Zuerich
       -
         ins: D. Hausheer
         name: David Hausheer
         org: OVGU Magdeburg
       -
         ins: D. Roos
         name: Dominik Roos
         org: Anapaya Systems
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
We first start from core components, that form a SCION minimal stack. We then move onto extensions and additional components, some of which provide compatibility mechanisms between SCION and existing protocols.

Before reading this document, please refer to {{DEKATER2022}} for a generic overview of SCION and its components, the problems it solves, and existing deployments. For an in-depth description of SCION, please refer to {{CHUAT22}}.

## Conventions and Definitions

{::boilerplate bcp14-tagged}

# Minimal stack - core components
In order to establish end to end connectivity, SCION relies on three main components.
SCION's data plane carries out secure path-aware forwarding. Its control plane takes case of routing. SCION relies on the Control Plane PKI to handle cryptographic material.

The control plane is responsible for discovering and disseminating routing information. Route discovery is performed by each autonomous system (AS) thanks to an authenticated path-exploration mechanism called beaconing.
SCION end hosts query their respective AS control plane and obtain authenticated and authorized network paths, in the form of path segments.
End hosts select one or more of the end to end network paths, based on the application requirements (i.e., latency). End hosts then craft SCION packets containing the end-to end path to the destination.
The data plane is responsible for forwarding SCION packets while authenticating them at each hop and.

Both the control and data plane rely on the control-plane PKI for authentication and authorization.
SCION's authentication mechanisms aim at protecting the whole end to end path at each hop. SCION Autonomous systems are organised in Isolation Domains (ISDs), that independently define their own roots of trust.
ISD members share an uniform trust environment (i.e., a common jurisdiction).
They can transparently define trust relationships between parts of the network by deciding wether to trust other ISDs.
SCION therefore relies on an unique trust model, which is markably different from other PKI. We clarify the motivation behind this in [Authentication](#pki)

All above mentioned core components are deployed in production (i.e., they are in use within the the SSFN, the Swiss Finance Network).
There are commercial implementations of all core components (including a high performance data-plane).

## Routing - Control Plane
The SCION control plane's main purpose is to discover and disseminate routing information, in the form of path segments.
Path exploration is based on path-segment construction beacons (PCBs), that are initiated by a subset of ASes and accumulate cryptographically protected path forwarding information. Each AS selects a few PCBs and makes them available to end hosts via its path service.
End hosts query the control plane for path segments, and combine them into forwarding paths to transmit packets in the data plane.
For an overview of the process to create and disseminate path information, refer to {{DEKATER2022}} section 1.2.2.

### Key properties in relationship to existing protocols
On a first sight, it might seem that SCION control plane takes care of similar duties as of BGP. While both focus on disseminating routing information, there are substantial differences in the properties provided and mechanisms. We describe the core properties provided by the SCION control plane, and its relationships with existing protocols.

- *Host addressing.*.  SCION decouples routing from end-host addressing, so inter-domain routing is based on ISD-AS tuples. SCION is agnostic to end-host addressing, therefore its control plane does not carry carry prefix information. SCION therefore can reuse existing end-host addressing mechanisms, as IPv6 or IPv4.

- *Multipath.* SCION ASes can select PCBs according to their policies, and register the corresponding path segments, making them available to other ASes and end hosts. SCION hosts can leverage a wide range of inter-domain paths, selecting them hop by hop based on application requirements or path conditions.
Another mechanism is BGP mutlipath {{RFC7911}}, focus on providing a backup path. However, it does not allow end hosts to select end to end path, and it faces scalability concerns  typical of BGP, as discussed in the above mentioned RFC.
Such concerns motivate an alternative approach as SCION.   

- *Hop by hop path authorization.* SCION packets can only be forwarded along authorized segments. This is achieved thanks to message authentication codes (MACs) within each hop field. During beaconing, each AS control's plane creates MACs, that are then verified at forwarding. This gives end hosts strong guarantees about the path where the data is routed. Other approaches, as BGPSec ({{RFC8205}}), suffer from challenges with scalability, and introduce circular dependencies [137] and global kill switches [441]
TODO: if we keep this, add citations from book

- *Scalability.* SCION beaconing algorithm is around two orders of magnitude more efficient than BGP due to the following reasons: the routing process is divided in a process within each ISD and one inter-ISD, SCION beaconing does not need to iteratively converge, SCION makes AS-based announcements instead of BGP’s prefix-based announcements. Please refer to {{KRAHENBUHL2022}} for an in-depth study of SCION's scalability.

- *Convergence time.* Since routing decisions are decoupled from dissemination of path information, SCION does not suffer from the long convergence times that affect path-vector protocols such as BGP.
Path information is propagated across the network by PCBs in times that are within the same order of magnitude of network round trip time.
This means that SCION has the capability to restore global reachability, even after catastrophic failures, in minutes.
In addition, in certain situations, BGP will never converge to a stable state, or converge only non-deterministically (see {{GRIFFIN1999}} and {{RFC4264}}.
  Convergence may also take too much time {{SAHOO2009}}.
TODO: Is SCION immune form such issues (as there is no convergence)?

- *Transparency.* SCION end-hosts have full visibility about the inter-domain path their data is forwarded. This is a property that is missing in traditional IP networks, where have no visibility nor guarantees on where their traffic is forwarded. SCION makes it harder to redirect traffic through an adversary's vantage point.

- *Fault isolation.* As the SCION routing process is divided in intra-ISD and inter-ISD, faults can have a more limited impact.
On the other hand, a single faulty BGP speaker can adversely impact routing globally.
TODO: I would be a bit more precise: what kind of fault would be contained? A path service going nuts or being compromised? And BGP is bad, but maybe we should mention that some of the issues (like hijacking) are mitigated by RPKI.  


- *Authenticated control messages.* BGP has no built-in security mechanisms and does not provide any tools for ASes to authenticate the information they receive through BGP update messages. This opens up a multitude of attack opportunities. SCION control messages, instead, are all authenticated.
In addition, SCION comprises the SCION Control Message Protocol (SCMP), which  is analogous to the Internet Control Message Protocol (ICMP). It provides functionality for network diagnostics, such as ping and traceroute, and error messages that signal packet processing or network-layer problems.
TODO: I'm not sure how much I want to go into SCMP here.. Especially as SCMP packets are only authenticated if DRKey/SPAO are used

The SCION control plane is dependent on the control-plane PKI {{#pki}} for authenticating control information.
TODO: Maybe we could go into more detail (i.e. verifying a path with CP certificates?) Maybe we can do this in the PKI section?


## Forwarding - Data plane

- *Path selecction* is made by end hosts, not routers
- **Scalability**
The use of forwarding tables in IP routers is time-consuming, expensive, and energy-intensive. Also, the constantly growing size of forwarding tables causes storage problems. Additionally, routers that keep state for network information can suffer from denial-of-service (DoS) attacks exhausting the router’s state {{SCHUCHARD2011}}.

- *Recovery from failure*
TODO: rewrite text
BGP only allows the selection of a single path to a destination. But having a multi-path choice can be welcome in several situations, e.g., in the case of a link failure, for load balancing, or when traffic is routed based on different policies.


###  SCION and Segment Routing

## Authentication -  SCION PKI {#pki}
TODO: why do we need a strong PKI?
* Talk about monopoly vs oligopoly and why this is important (but maybe in the CP part)?
* Why we could not just use RPKI 9that we use for origin validation)
This makes the SCION CP-PKI distinct from other PKIs (i.e. web PKI, RPKI), that either have a single root of trust root (monopoly model), or rely on a plethora of roots of trust (oligopoly model) leading to a trust architecture that supports meaningful trust roots in a global environment with inherently distrustful entities.

*  Absence of Kill Switches
Monopolistic trust root architectures such as DNSSEC and RPKI/BGPsec en- able entities in possession of private keys to shut down portions of the names- pace controlled by those keys. The introduction of these kill switches into DNS and BGP has created skepticism and concern over the potential outages that could arise should private keys be misused or fall into the wrong hands [441].

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
