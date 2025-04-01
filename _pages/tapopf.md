---
permalink: /tapopf21/
title: "IEEE TaPoPF Workshop"
excerpt: "TaPoPF '21"
redirect_from: 
  - /tapopf21.html
layout: external
---
{% include base_path %}

## 1st IEEE Workshop on Theory and Practice of Programmable Forwarding

June 28th, 2021 <br />
Co-located with IEEE Netsoft 2021

## Call for Papers

Over the past decade, computer networks have been transformed into an end-to-end programmable platform. Early work on SDN largely focused on on the control plane, but more recent efforts on NFV, P4, etc. have also made the forwarding plane programmable. Hence, for the first time, network owners now have full control over the software executing in their networks. The question then becomes: what should they do with this new-found capability? 

We seek technical contributions on the following topics:

* **Programming Models:** What are good models for programming the forwarding plane? Many software targets utilize general-purpose languages such as eBPF or DPDK. But these languages are hard to map down to hardware targets. Conversely, many hardware targets utilize domain-specific languages such as P4 or NPL. But these languages are computationally restricted and cannot express complex network functions that make significant use of state. Is there a way to combine the best of both approaches? 

* **Hardware Platforms:** With the end of Moore's Law and ever-increasing links speeds, the need for programmable hardware seems inevitable. Cloud providers are already equipping physical hosts with hardware accelerators based on FPGAs or SmartNICs -- a trend that is likely to continue. What are promising architectures for packet processing in hardware? What are the key trade offs, and how can we balance flexibility, efficiency, predictability, and performance?

* **Applications:** Early programmable forwarding platforms were mostly used to implement custom protocols or simple enhancements like in-band network telemetry. But the community has also started to explore ideas such as in-network computing, systems in which algorithms traditionally realized in the control plane are instead pushed into the data plane, and even forms of active networking. What is the right division of labor between the control plane and the data plane? Between the network and end hosts? How can we utilize programmability to enhance traditional network services such as congestion control. And what are techniques for realizing sophisticated algorithms on resource-limited devices?

* **Verification:** The emergence of programmable forwarding has been matched by growing interest in network verification. Intuitively, if networks are specified in software, then we should be able to use traditional program verification techniques to reason about networks behavior. Indeed, researchers have developed scalable techniques for reasoning about network control planes and data planes. The next questions are how we can use these newfound reasoning capabilities to address security and reliability issues.

The goal of this workshop is to bring together a diverse group of researchers and practitioners to discuss recent research results and identify future challenges related to programmable forwarding. We welcome technical contributions of all kinds including papers discussing new approaches, experience reports, tools, surveys, demos, etc.

## Technical Program Committee
- Akihiro Nakao, University of Tokyo (Co-Chair)
- Nate Foster, Cornell University and Barefoot Networks (Co-Chair)
- Ping Du, University of Tokyo
- Anja Feldmann, Max Planck Institute 
- Xin Jin, Johns Hopkins
- Yuliang Li, Google
- Hongqiang Liu, Alibaba

## Important Dates

- Paper Submission: March 5, 2021
- Notification of Acceptance: March 28, 2021
- Camera-ready: April 11, 2021
- Workshop date: June 28, 2021

## Paper Submission

Authors are invited to submit original contributions (written in English) in PDF format. Only original papers not published or submitted for publication elsewhere can be submitted. Papers should be up to 7 pages excluding 1 page of references in IEEE 2-column US-Letter style using IEEE Conference template and submitted in PDF format via:

[https://edas.info/N28100](https://edas.info/N28100)
