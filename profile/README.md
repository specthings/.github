The *specthings* project provides a customizable data format, software
components, and command line tools to specify, describe, document, and build
things.

The primary use case for this projects is supporting software development
according to two standards published by the
[European Cooperation for Space Standardization (ECSS)](https://ecss.nl/):

* [ECSS-E-ST-40C Rev.1 - Software (30 April 2025)](https://ecss.nl/standard/ecss-e-st-40c-rev-1-software-30-april-2025/)
* [ECSS-Q-ST-80C Rev.2 - Software product assurance (30 April 2025)](https://ecss.nl/standard/ecss-q-st-80c-rev-2-software-product-assurance-30-april-2025/)

Support for other software development standards can be added on demand.

The specification items for software and the utilities provided by *specware*
and *specbuild* enable you to:

* specify a software product
* write validation tests
* run software tests
* gather, evaluate and present test results
* gather, evaluate and present code and branch coverage information
* gather, evaluate and present software performance measurements
* produce a Technical Specification (TS) consisting an Interface Control Document (ICD) and a Software Requirements Specification (SRS)
* produce software design and architecture documents
* produce software product assurance documents
* produce user manuals
* produce test plan documents
* produce test report documents
* provide traceability from the specification, to the software design, to the source code, to test plans, to test results, and vice versa
* run static code analysers, present the results, provide links to results in other documents
* build the tools used to build the software product
* build the software product
* package everything as an archive file
* produce a Software Configuration File (SCF) describing the package

The components of *specthings* are:

* *specitems*:
  Provides interfaces to work with specification items.  Specifications are
  written in specification items which may contain dictionaries, lists,
  integers, floating-point numbers, and strings.  The format of these items is
  extensible, human readable, machine readable, Git friendly, and can be
  customized according to domain-specific needs.  The items are connected
  through links which may contain role-specific extra information.  This
  enables different views to a specification item graph depending on the use
  case.
* *specware*:
  Provides utilities to specify software and generate source code for
  interfaces and validation tests from the specification.

* *specbuild*:
  Provides utilities to build packages of software products along with their
  documentation.
