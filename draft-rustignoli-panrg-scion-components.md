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
  RFC5880:
  RFC8402:
  RFC5280:
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
  I-D.dekater-scion-overview:
    title: SCION Overview
    date: 2022
    target: https://datatracker.ietf.org/doc/draft-dekater-panrg-scion-overview/
    author:
      -
        ins: C. de Kater
        name: Corine de Kater
        org: ETH Zuerich
      -
        ins: N. Rustignoli
        name: Nicola Rustignoli
        org: ETH Zuerich
      -
        ins: A. Perrig
        name: Adrian Perrig
        org: ETH Zuerich

  I-D.garciapardo-drkey:
    title: Dynamically Recreatable Keys
    date: 2022
    target: https://datatracker.ietf.org/doc/draft-garciapardo-panrg-drkey/
    author:
      -
        ins: 	J. Pardo
        name: Juan A. García Pardo Giménez de los Galanes
        org: ETH Zuerich
      -
        ins: C. Krähenbühl
        name: Cyrill Krähenbühl
        org: ETH Zuerich
      -
        ins: B. Rothenberger
        name: Benjamin Rothenberger
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
  SUPRAJA2021:
    title: "Global Distributed Secure Mapping of Network Addresses"
    date: 2021
    target: https://netsec.ethz.ch/publications/papers/sridhara_taurin2021_siam.pdf
    author:
      -
        ins: S. Supraja
        name: Supraja Sridhara
        org: ETH Zuerich
      -
        ins: F. Wirz
        name: François Wirz
        org: ETH Zuerich
      -
        ins: J. de Ruiter
        name: Joeri de Ruiter
        org: SIDN Labs
      -
        ins: C. Schutijser
        name: Caspar Schutijser
        org: SIDN Labs
      -
        ins: M. Legner
        name: Markus Legner
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

Before reading this document, please refer to {{I-D.dekater-scion-overview}} for a generic overview of SCION and its components, the problems it solves, and existing deployments. For an in-depth description of SCION, please refer to {{CHUAT22}}.

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
For an overview of the process to create and disseminate path information, refer to {{I-D.dekater-scion-overview}} section 1.2.2.


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


- *Authenticated control messages.* BGP has no built-in security mechanisms and does not provide any tools for ASes to authenticate the information they receive through BGP update messages. This opens up a multitude of attack opportunities. SCION control-plane messages, instead, are all authenticated.
In addition, currently the Internet Control Message Protocol (ICMP) lacks an authenticated counterpart, see {{RFC4443}} and {{RFC0791}}. Unauthenticated ICMP messages can potentially be used to affect or even prevent traffic forwarding.
SCION provides the SCION Control Message Protocol (SCMP), which  is analogous to ICMP. It provides functionality for network diagnostics, such as ping and traceroute, and error messages that signal packet processing or network-layer problems. SCMP is the first control message protocol supports the authentication of network control messages.
TODO: I'm not sure how much I want to go into SCMP here.. Especially as SCMP packets are only authenticated if DRKey/SPAO are used

The SCION control plane is dependent on the control-plane PKI (#pki) for authenticating control information.
TODO: Maybe we could go into more detail (i.e. verifying a path with CP certificates?) Maybe we can do this in the PKI section?

TODO: add a few sentences on why the CP avoids mistakes in lessons learned from RFC9049

## Forwarding - Data plane
SCION is an inter-domain network architecture and as such does not interfere with intra-domain forwarding. This corresponds to the general practice today where BGP and IP are used for inter-domain routing and forwarding, respectively, but ASes use an intra-domain protocol of their choice, (i.e., OSPF or IS-IS for routing and IP, MPLS, SR and various layer-2 protocols for forwarding).
SCION therefore re-uses the intra-domain network fabric to provide connectivity among its infrastructure services, border routers, and end hosts, minimising changes to the internal infrastructure.

SCION routers are deployed at the network edge. They receive and validate SCION packets from neighbours, then they use their intra-domain forwarding information to transmit packets to the next border router or SCION end-host.

SCION packets sit at network-layer (layer-3), and the SCION header sits between the transport-layer (layer-4) and link-layer (layer-2). They contain a variable type and length end-host address, and can therefore carry any address (IPv4, IPv6, ...). In addition, ed host addresses only need to be unique within an AS, and can be, in principle, reused.
In early deployments, intra-AS SCION packets are sometimes encapsulated into an IP packet, for backwards compatibility.

### Key properties in relationship to existing protocols
Thanks to its data plane, SCION achieves properties that are difficult to achieve when exclusively extending existing protocols.

- *Programmable paths.* SCION end hosts select network paths based on application requirements, rather than routers.
This approach is such that there is no need to include semantics in packets, as routing decisions are left to end hosts. In addition, when comparing to proposed semantic routing (TODO: reference) approaches, with SCION  hosts gain better visibility into network paths.
TODO: I'm not sure if we want to explicitly say that this approach has advantages to semantic routing.. Maybe we don't want to mention it?
https://www.ietf.org/id/draft-farrel-irtf-introduction-to-semantic-routing-04.html#I-D.king-irtf-semantic-routing-survey
TODO: @Adrian, I remember you don't like the expression "programmable paths".. Anything better? "Path selection"?

- **Scalability.**
SCION routers can efficiently forward packets without the need to look up forwarding tables and without keeping per-connection state. Routers only need to verify  MACs in hop fields. This operation is based on modern block ciphers such as AES, can be computed faster than performing a memory lookup and it is widely supported in modern CPUs.
Routers, therefore, do not require expensive and energy-intensive dedicated hardware, and can  be deployed on off-the-shelf hardware. Lack of forwarding tables also implies that the growing size of forwarding tables is of no concern. Additionally, routers that keep state for network information can suffer from denial-of-service (DoS) attacks exhausting the router’s state {{SCHUCHARD2011}}.

- *Recovery from failures.*
SCION hosts usually receive more than one path to a given destination.
Each host can select (potentially disjoint) backup paths that are readily available in case of failure.
In contrast to the IP Internet, SCION packets are not dynamically rerouted in the network in case of failures. Routers use BFD {{RFC5880}} to detect link failures, and in case they cannot forward a packet they send an authenticated SCMP message triggering path revocation. End hosts can use this information, or alternatively active monitoring, to quickly reroute trafifc in case of failures.
There is therefore no need to wait for BGP convergence.

- *Extensibility* SCION, similarly to IPv6, supports extensions in its header.
Such extensions can be hop-by-hop and end-to-end.

- *Backwards compatibility.* SCION packets support any kind of end-host addressing. IP packets can therefore be transported over SCION by interposing a SCION to IP Gateway (SIG). TODO: reference if we talk more about it later.



###  SCION and Segment Routing
Given its path-aware properties, some of SCION's characteristics might seem similar to the ones provided by Segment Routing (SR) {{RFC8402}}. There are, however, fundamental differences that distinguish and motivate SCION.
The most salient one is that Segment Routing is designed to be deployed across a single trusted domain. SR therefore does not focus on security, which remains an open question. SCION, instead, is designed from inception to allow inter-domain communication between mutually distrustful entities.
It comes, therefore, with an arsenal of tools to prevent attacks (i.e., authenticating all control plane messages and all critical fields in the data-plane header).
Rather than competing, SCION and SR could potentially complement each other. SCION relies on existing intra-domain routing protocols, therefore SR could represent one of the possible intra-domain routing protocols. Possible integration of their path-aware properties remain for now an open question.

TODO: Maybe cite https://datatracker.ietf.org/doc/draft-li-spring-srv6-security-consideration/


## Authentication -  SCION PKI {#pki}
SCION's control plane messages are all authenticated. The verification of those messages relies on a public-key infrastructure (PKI) called the control-plane PKI or CP-PKI.
It consists of a  set of mechanisms, roles, and policies related to the management and usage of certificates, which enable the verification of signatures, e.g., on path construction beacons (PCBs).
One might ask why SCION requires its own PKI, rather than reusing some of the existing PKI architectures. There are several properties that distinguish the CP-PKI from others, and motivate SCION's distinct approach.

*Unique decentralised trust model*. SCION is designed to enable global secure connectivity, where ASes do not necessarily share mutual trust.
This requires a trust model that is different from existing ones that are behind commonly deployed PKIs in today's Internet.
In a monopolistic model, all entities trust a single root of trust (e.g., in DNSSEC). In an oligopolistic model, there are  multiple equally trusted roots  (e.g., in the Web PKI).
In both models, some or all certification authorities are omnipotent. If their key is compromised, then the security of the entire system collapses.
Both models do not scale well to a global environment, because mutually distrustful entities cannot agree on a single root of trust (monopoly) and because in the oligopoly model, the security is as strong as its weakest root.
The SCION trust model differs from classic PKIs in two ways. First, no entity is omnipotent, as  Isolation Domains  elect their own root of trust, and the  capabilities of each ISDs (authentication-wise) are limited to communication channels in which they are involved. Second, the trust roots of each ISD are co-located in a single file, the TRC, which is co-signed by multiple entities in a process  called voting.


- *Absence of global  kill switches*. Authentication relies on local trust roots, limiting the scope of authorities and offering local sovereign.
Monopolistic trust root architectures such as DNSSEC and RPKI/BGPsec enable entities in possession of private keys to shut down portions of the namespace controlled by those keys. The introduction of these kill switches into DNS and BGP has created skepticism and concern over the potential outages that could arise should private keys be misused or fall into the wrong hands [441].
In addition, during periods of global tensions, there are often calls to use some of today’s Internet kill switches to potentially shut down connectivity in portions of the Internet. IN SCION, the fact that each ISD can manage its own roots of trust independently, prevents such external kill switches.
TODO: add citation 441

- *Resilience to compromised entities and keys.* Compromised or malicious trust roots outside an ISD cannot affect operations that stay within that ISD. Moreover, each ISD can be configured to withstand the compromise of any single voting key.

- *Trust flexibility*: Each ISD can define its own trust policy. ASes must accept the trust policy of the ISD(s) in which they participate, but they can decide which ISDs they want to join, and they can participate in multiple ISDs.

- *Scalability*: The authentication infrastructure scales to the size of the Internet and is adapted to the heterogeneity of today’s Internet constituents.

- *A basis for authentication of data-plane messages*.  Authentication based on digital signatures works well for the relatively low message rates in the control plane, but it does not meet the performance requirements for the high message rate of the data plane.
The authentication of data-plane traffic and control messages requires a highly efficient and ideally stateless system to achieve bandwidths of several Gbps on commodity hardware, and to avoid creating opportunities for DoS attacks.
SCION comprises a component called  DRKey, which enables high-speed data-plane components, like border routers, to derive symmetric cryptographic keys from local secrets only. Such component is used to authenticate SCMP messages.
Today's Internet also lacks a fundamental mechanism to share a secret key between two end hosts for secure end-to-end communication. Existing approaches (i.e., SSH) resort to trust-on-first-use (TOFU) approach, where an host's initial public key is accepted without verification. DRKey addresses such issue.
For more information, refer to the draft {{I-D.garciapardo-drkey}}.

The CP-PKI is based on certificates that follow the X.509v3 standard {{RFC5280}}. There are several professional industry-grade implementations, e.g., by SIX, the main financial infrastructure and service provider in Switzerland.
Trust within an ISD is normally bootstrapped with an initial ceremony. Subsequent updates to the root of trust are handled automatically.

### SCION and RPKI
One might ask why SCION could not just rely on RPKI. Summarising on the points above, the CP-PKI distinguishes itself because of the trust model, which comprises independent trust roots that are a fundamental building block for SCION's Isolation Domains.
RPKI's trust model follows the same structure as the IP allocation hierarchy, where the five RIRs run a CA. This  clashes with the trust model required for SCION's Isolation Domains.
In addition, RPKI is only meant to provide authorisation, but not authentication.
SCION indeed does not provide, by design, IP authorisation. Rather, as we further describe in the next section, one of  IP to SCION's  coexistence mechanisms (SIAM) relies on RPKI for IP origin attestation.

# Transition mechanisms
As we presented in {{I-D.dekater-scion-overview}}, SCION comprises multiple transition mechanisms that allow an incremental deployment and coexistence with existing protocols.
Such approaches require different level of changes in existing systems, and have different maturity levels (from research to production).
Rather than describing how each mechanism works, we provide a short summary of the approach, focusing on what its functions, properties, and protocols it reuses, extend or interact with.

-  *SCION-IP-Gateway (SIG)*.  A SCION-IP-Gateway (SIG) encapsulates regular IP packets into SCION
   packets with a corresponding SIG at the destination that performs the
   decapsulation.
   This mechanism enables legacy IP end hosts to benefit from a SCION deployment by transparently obtaining improved security and availability properties.
   SCION routing policies can be configured on SIGs, in order to selsect appropriate SCION paths based on application requirements.
   SIGs have the ability to dynamically exchange prefix information, currently using their own encapsulation and prefix exchange protocol. This does not exclude reusing existing protocols in the future.
   SIGs are deployed in production SCION networks, and there are commercial implementations.

- *SIAM*. To make SIGs a viable transition mechanism in an Internet-scale network with tens of thousands of ASes, an automatic configuration system is required. SIAM creates mappings between legacy IPs and SCION addresses, relying on the authorisations in the Resource Public Key Infrastructure (RPKI). SIAM  is currently a research prototype, further described in {{SUPRAJA2021}}.

- *SBAS* is an experimental architecture aiming at extending benefits of SCION (in terms of performance and routing security) to potentially any IP host on the Internet.
SBAS consists of a federated backbone of entities. SBAS appears on the outside Internet as a regular BGP-speaking AS. Customers of SBAS can leverage the system to route traffic across the SCION network according to their requirements (i.e., latency, geography, ... ). SBAS contains globally distributed PoPs that advertise its customer's announcements. Traffic is therefore routed as close as possible to the source onto the SCION network. The system is further described in chapter 13 of {{CHUAT22}}.
TODO: I find it very difficult to explain SBAS in a few lines... It is quite a big system and I'm not so sure we should talk about it. I'm afraid it might distract the focus.


# Additional components
TODO: Add some description
- Happy eyeballs (and how we extend it)
- DrKey & dependencies --> {{I-D.garciapardo-drkey}}
  - LightningFilter --> https://datatracker.ietf.org/meeting/111/materials/slides-111-panrg-lightning-filter-high-speed-traffic-filtering-based-on-drkey
  - SCMP
- COLIBRI (Bandwidth Reservations)
- End-host stack
- *RHINE* (formerly RAINS)


# Dependency analysis
This section briefly discusses dependencies between SCION's core components, with the goal of facilitating a discussion on standardization.
TODO: this section contains just notes, to be rephrased

- Only PKI - authentication: Overall, the PKI, with its trust model, constitutes the most independent unit that could be potentially  be leveraged by SCION and other protocols. The PKI itself does not have significant dependencies on other pieces, therefore a good starting point would be to describe its trust properties, inrerfaces, and processes.

- Only control plane - beaconing & path server infrastructure
  The SCION control plane relies on the CP-PKI to authenticate entities. It would therefore make sense to define the CP in parallel with PKI. Decoupling it from PKI would severely affect the properties and guarantees that can be provided by the CP

- Only data plane - path construction and packet forwarding
  DP needs a way to authenticate path information.. If not, it would not make sense to have SCION for inter-domain.. We would just mimick SR and it would be useless on inter-domain, where the trust model is different. As discussed in {{RFC9049}}, lack of authentication has often been the cause of some protocols never taking off because of security concerns (see Section 6.5 (Trigtran),  6.7 (NSIS) of the mentioned draft. )


- Only other components (i.e., SCMP)
  TODO



# Conclusions
We described key SCION components with their properties and dependencies.
TODO: I would add some comments on how SCION avoids some of the issues mentioned in {{RFC9049}}
Also mention that the most important core components are formally verified.



# Security Considerations

TODO Security


# IANA Considerations

This document has no IANA actions.


--- back

# Acknowledgments
{:numbered="false"}

We are also indebted to Laurent Chuat,
Markus Legner, David Basin, David Hausheer, Samuel Hitz, and Peter
Mueller, for writing the book "The Complete Guide to SCION"
[CHUAT22], which provides the background information needed to write
this informational draft.
