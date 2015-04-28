---
layout: page
title: Research
permalink: /research/
---


**Advisors**: [José Carlos Maldonado](http://lattes.cnpq.br/8807333466702951) - [Paulo Meirelles](http://lattes.cnpq.br/2193972715230641)


# Theme

Use of middlewares to reduce coupling between integration server and integrated applications


# Problem

Usuallly software development process of integrated applications, in general, require modifications in each of the integrated tools (or services). In Open-Source that leads the developers to maintain their own forks of each tool that composes the system. That's an intrinsic problem of high coupling between components.


# Research Question

How to reduce coupling between integration server and integrated applications in Web context?


# Hypothesis

The use of plugable middlewares in the application server will reduce coupling between the aplication server and the integrated services.


# Goals

Confirming the hypothesis, the goal is to develop a reference architecture of an integration server with better control under coupling between integrated applications and integration servers.


# Abstract

Integration servers usually concentrates all relevante code and data to allow
the integrated applications to communicate and in many cases the applications
also need to be modified in order to reply to the integration server messages,
increasing coupling and reducing the manutenability. If application servers
could communicate with plugable middlewares and the middlewares could pass the
messages over to the application then the application server would have no
direct interaction with the application itself and with that, we expect
coupling between systems to deacrease and though manutenability to increase
as result.


# Literature

* [Why is the web loosely coupled?: a multi-faceted metric for service design](http://dl.acm.org/citation.cfm?id=1526832)

* [Coupling Metrics for Predicting Maintainability in Service-Oriented Designs](http://ieeexplore.ieee.org/xpls/abs_all.jsp?arnumber=4159685)
