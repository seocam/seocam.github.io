---
layout: page
title: Research
permalink: /research/
---

# Theme

Use of middlewares to reduce coupling between integration server and integrated applications


# Problem

How to reduce coupling between integration server and integrated applications in Web context?


# Hypothesis

Using plugable middlewares in the application server will reduce coupling between the aplication server and the integrated services.


# Justification / Motivation

Integration servers usually concentrates all relevante code and data to allow
the integrated applications to communicate and in many cases the applications
also need to be modified in order to reply to the integration server messages.

If application servers could communicate with plugable middlewares and
the middlewares could pass the messages over to the application then the
application server would have no direct interaction with the application
itself. Also, in order to allow applications react to other application events the
middlewares would need to be able to listen, fire and propagate event signals.


# Literature

* [An Introduction to Software Architecture](http://repository.cmu.edu/compsci/724/?utm_source=repository.cmu.edu%2Fcompsci%2F724&utm_medium=PDF&utm_campaign=PDFCoverPages)

* [Why is the web loosely coupled?: a multi-faceted metric for service design](http://dl.acm.org/citation.cfm?id=1526832)

* [Coupling Metrics for Predicting Maintainability in Service-Oriented Designs](http://ieeexplore.ieee.org/xpls/abs_all.jsp?arnumber=4159685)
