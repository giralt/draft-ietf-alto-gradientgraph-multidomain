---
###
# Internet-Draft Markdown Template
#
# Rename this file from draft-todo-yourname-protocol.md to get started.
# Draft name format is "draft-<yourname>-<workgroup>-<name>.md".
#
# For initial setup, you only need to edit the first block of fields.
# Only "title" needs to be changed; delete "abbrev" if your title is short.
# Any other content can be edited, but be careful not to introduce errors.
# Some fields will be set automatically during setup if they are unchanged.
#
# Don't include "-00" or "-latest" in the filename.
# Labels in the form draft-<yourname>-<workgroup>-<name>-latest are used by
# the tools to refer to the current version; see "docname" for example.
#
# This template uses kramdown-rfc: https://github.com/cabo/kramdown-rfc
# You can replace the entire file if you prefer a different format.
# Change the file extension to match the format (.xml for XML, etc...)
#
###
title: "Bottleneck Structure Graphs in Multidomain Networks: ALTO Use Cases and Requirements"
category: info

docname: draft-giraltyellamraju-alto-bsg-multidomain-latest 
ipr: trust200902
area: Application
workgroup: ALTO
keyword: ALTO
venue:
  group: WG
  type: Working Group
  mail: alto@ietf.org
  arch: https://mailarchive.ietf.org/arch/browse/alto/
  github: giralt/draft-ietf-alto-gradient-graph
  latest: https://giralt.github.io/draft-ietf-alto-gradient-graph/draft-giraltyellamraju-alto-bsg-requirements.html

stand_alone: yes
smart_quotes: no
pi: [toc, sortrefs, symrefs]

author:
 -
    name: Jordi Ros-Giralt
    organization: Qualcomm
    email: jros@qti.qualcomm.com
 -
    name: Sruthi Yellamraju
    organization: Qualcomm
    email: yellamra@qti.qualcomm.com
 -
    name: Qin Wu
    organization: Huawei
    email: bill.wu@huawei.com
 -
    name: Luis Miguel Contreras
    organization: Telefonica
    email: luismiguel.contrerasmurillo@telefonica.com
 -
    name: Richard Yang
    organization: Yale University
    email: yry@cs.yale.edu
 -
    name: Kai Gao
    organization: Sichuan University
    email: kaigao@scu.edu.cn


normative:
  RFC7285:
  RFC8402:
  RFC8896:
  I-D.ietf-alto-path-vector:
  I-D.ietf-alto-performance-metrics:

informative:

  G2-SIGMETRICS:
    title : On the Bottleneck Structure of Congestion-Controlled Networks
    seriesinfo : ACM SIGMETRICS
    author:
      -
        ins: J. Ros-Giralt
        name: Jordi Ros-Giralt
        org: Reservoir Labs / Qualcomm
      -
        ins: A. Bohara
      -
        ins: S. Yellamraju
      -
        ins: H. Langston
      -
        ins: R. Lethin
      -
        ins: Y. Jiang
      -
        ins: L. Tassiulas
      -
        ins: J. Li
      -
        ins: Y. Tan
      -
        ins: M. Veeraraghavan
    date: 2020

  G2-SIGCOMM:
    title : Designing data center networks using bottleneck structures
    seriesinfo : ACM SIGCOMM
    author:
      -
        ins: J. Ros-Giralt
        name: Jordi Ros-Giralt
        org: Reservoir Labs
      -
        ins: N. Amsel
      -
        ins: S. Yellamraju
      -
        ins: J. Ezick
      -
        ins: R. Lethin
      -
        ins: Y. Jiang
      -
        ins: A. Feng
      -
        ins: L. Tassiulas
      -
        ins: Z. Wu
      -
        ins: K. Bergman
    date: 2021


  G2-TREP:
    title : A Quantitative Theory of Bottleneck Structures for Data Networks
    seriesinfo : Reservoir Labs (Qualcomm) Technical Report
    author:
      -
        ins: J. Ros-Giralt
        name: Jordi Ros-Giralt
        org: Reservoir Labs
      -
        ins: N. Amsel
      -
        ins: S. Yellamraju
      -
        ins: J. Ezick
      -
        ins: R. Lethin
      -
        ins: Y. Jiang
      -
        ins: A. Feng
      -
        ins: L. Tassiulas
      -
        ins: Z. Wu
      -
        ins: K. Bergman
    date: 2021


  G2-SC:
    title : Computing Bottleneck Structures at Scale for High-Precision Network Performance Analysis
    seriesinfo : IEEE International Workshop on Innovating the Network for Data Intensive Science (INDIS), Supercomputing
    author:
      -
        ins: N. Amsel
        name: Noah Amsel
        org: Reservoir Labs
      -
        ins: J. Ros-Giralt
      -
        ins: S. Yellamraju
      -
        ins: B. von Hoffe
      -
        ins: R. Lethin
    date: 2020


  LORENZ:
    title : Does the flap of a butterfly's wings in Brazil set off a tornado in Texas?
    seriesinfo : American Association for the Advancement of Science, 139th Meeting
    author :
      -
        ins: E. Lorenz
    date : 1972

  GALLAGER:
    title : "Data Networks"
    date: 1992
    author :
      -
        ins: R. Gallager
      -
        ins: D. Bertsekas

  B4-SIGCOMM :
    title : "B4: Experience with a Globally-Deployed Software Defined WAN"
    author :
      -
        ins: S. Jain et al
    date : 2013
    seriesinfo : "ACM SIGCOMM"

  BE-SIGCOMM :
    title : "BwE: Flexible, Hierarchical Bandwidth Allocation for WAN Distributed Computing"
    author :
      -
        ins: A. Kumar et al
    date : 2015
    seriesinfo : "ACM SIGCOMM"

  SH-SIGCOMM :
    title : "Cost-effective capacity provisioning in wide area networks with Shoofly"
    author :
      -
        ins: R. Singh et al
    date : 2021
    seriesinfo : "ACM SIGCOMM"

  PETERSON :
    title : "5G Mobile Networks: A Systems Approach"
    author :
      -
        ins: L. Peterson
      -
        ins: O. Sunay
    date : 2020
    seriesinfo : "Open Networking Foundation"

  MMSYS :
    title : "Bandwidth Estimation for Real-Time Communications"
    target : https://2021.acmmmsys.org/rtc_challenge.php
    date : 2021


  BE-ONL :
    title : "Bandwidth Estimation on OpenNetLab"
    target : https://datatracker.ietf.org/meeting/112/materials/slides-112-alto-bandwidth-estimation-service-00
    seriesinfo : "IETF Plenary 112, IETF ALTO WG"
    date : 2021

  FLOWDIR :
    title : "Steering Hyper-Giants' Traffic at Scale"
    author :
      -
        ins: E. Pujol
        name: Enric Pujol
        org: BENOCS
      -
        ins: I. Poese
      -
        ins: J. Zerwas
      -
        ins: G. Smaragdakis
      -
        ins: A. Feldmann
    seriesinfo : "ACM CoNEXT"
    date : 2019

  JSP-INFOCOM :
    title : "Joint Service Placement and Request Routing in Multi-cell Mobile Edge Computing Networks"
    author :
      -
        ins: D. Poularakis et al
        org: Yale University

  NOVA:
    title : An objective-driven on-demand network abstraction for adaptive applications
    seriesinfo :
      IEEE/ACM: "IEEE/ACM Transactions on Networking (TON) Vol 27, no. 2 (2019): 805-818."
    target : https://doi.org/10.1109/IWQoS.2017.7969117
    author :
      -
        ins: K. Gao
      -
        ins: Q. Xiang
      -
        ins: X. Wang
      -
        ins: Y. Yang
      -
        ins: J. Bi
    date: 2019

  MERCATOR:
    title : Toward Fine- Grained, Privacy-Preserving, Efficient Multi-Domain Network Resource Discovery
    seriesinfo :
      IEEE/ACM:  "IEEE/ACM IEEE Journal on Selected Areas of Communication 37(8): 1924-1940"
    target : https://doi.org/10.1109/JSAC.2019.2927073
    date : 2019
    author :
      -
        ins: Q. Xiang
      -
        ins: J. Zhang
      -
        ins: X. Wang
      -
        ins: C. Guok
      -
        ins: F. Le
      -
        ins: J. MacAuley
      -
        ins: H. Newman
      -
        ins: Y. Yang

  SINGULARITY-MSFT :
    title : "Singularity: Planet-Scale, Preemptive and Elastic Scheduling of AI Workloads"
    target : https://arxiv.org/pdf/2202.07848.pdf
    author :
      -
        ins: D. Shukla et al
        org: Microsoft

  TOPOOPT-MIT :
    title : "TOPOOPT: Optimizing the Network Topology for Distributed DNN Training"
    target : https://arxiv.org/pdf/2202.00433.pdf
    author :
      -
        ins: W. Wang et al
        org: MIT, Facebook, CMU, Telescent

  FLEXFLOW-STFORD :
    title : "Beyond Data And Model Parallelism For Deep Neural Networks"
    target : https://arxiv.org/pdf/1807.05358.pdf[
    author :
      -
        ins: Z. Jia et al
        org: Stanford


--- abstract

TODO Abstract


--- middle

# Introduction

TODO Introduction


# Conventions and Definitions

{::boilerplate bcp14-tagged}


# Security Considerations

TODO Security


# IANA Considerations

This document has no IANA actions.


--- back

# Acknowledgments
{:numbered="false"}

TODO acknowledge.
