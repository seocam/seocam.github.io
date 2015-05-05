---
layout: research
title: Research
permalink: /research/
---


# Use of Integration Middlewares to Increase Maintainability in Integrated Systems

**Advisors**: [José Carlos Maldonado](http://lattes.cnpq.br/8807333466702951) - [Paulo Meirelles](http://lattes.cnpq.br/2193972715230641)

## Context

There are cases where a single existing system does not meet a set of raised requirements. In those cases using a group of systems instead of just one it is an option but doing so also bring some drawbacks such as multiple user accounts, different user experience and duplicated information. To reduce the drawbacks the systems can be integrated into a new composed system.


## Problems and Gaps

The integration of independently designed and developed systems, in many cases, require modifications in each of the integrated parts. That occurs because the parts were not designed for integration but actually to serve specific purposes. In some cases where the source code is available the changes can be made by the integrators but in other cases the requirements need to be addressed to the company or people developing and maintaining it. None of the two scenarios are ideal because in both cases the modifications would impact system maintainability.

## Research Questions

How to build a system composed by integrated parts without compromise maintainability?


## Hypothesis

1. The use of an integration server with plugable middlewares will reduce coupling between parts and integration server increasing Maintainability.
1. The use of middlewares will impact system's Efficiency in an acceptable level (up to 5%).
1. The use of middlewares will improve the integration server Portability.


## Methods

The **ISO9126-3:2002** product quality metrics will be used to evaluate a real system in the following *Quality Attributes* and its subcharacteristics:

### Maintainability
* Analyzability
* Changeability
* Stability
* Testability
* Compliance


### Portability
* Adaptability
* Installability
* Co-existence
* Replaceability
* Compliance


### Efficiency
* Time behaviour
* Resource utilization
* Compliance


The *Quality Attributes* will be measured using the metrics described on the **ISO9126-3:2002** in two real integrated systems already in use: the *Software Público Brasileiro* (SPB) and *Interlegis' Colab* (IC). The systems were choosen because both are Open-Source and use the same integration server (called *Colab*), and one of then has with modifications directly on Colab's source code (IC) and the other uses middlewares (SPB). The applied metrics will result on absulute values from 0 to 1 for each subcharacteristic. Any score improvement will be considered for Maintainability and Portability and a loss up to 0.05 on Efficiency will be considered satisfactory.



## Abstract

Integration servers usually concentrates all relevante code and data to allow
the integrated applications to communicate and in many cases the applications
also need to be modified in order to reply to the integration server messages,
increasing coupling and reducing the maintainability. If application servers
could communicate with plugable middlewares and the middlewares could pass the
messages over to the application then the application server would have no
direct interaction with the application itself and with that, we expect
coupling between systems to deacrease and though maintainability to increase
as result.


## Literature

* [Why is the web loosely coupled?: a multi-faceted metric for service design](http://dl.acm.org/citation.cfm?id=1526832)

* [Coupling Metrics for Predicting Maintainability in Service-Oriented Designs](http://ieeexplore.ieee.org/xpls/abs_all.jsp?arnumber=4159685)




 The impact occur because when one part is changed the integration might be affected, for example, if a part A depends on a database schema on part B when that schema is altered part A will start to malfunction. The evolvability is also likely to be affected by an update because the new code can conflict with the patch applied for integration and this is aggravated by the fact that the integration team and developers from parts are working independently and thus did not coordinate the update.