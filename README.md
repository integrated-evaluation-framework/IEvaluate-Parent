# The *I*ntegrated *Evaluat*ion Framework [![Build Status](https://travis-ci.com/integrated-evaluation-framework/IEvaluate-Parent.svg?branch=master)](https://travis-ci.com/integrated-evaluation-framework/IEvaluate-Parent)
## Introduction

The ***I***ntegrated ***Evaluat***ion Framework (IEvaluate) provides a flexible, centralized platform for validating and 
monitoring artificial intelligence applications. Specifically, it provides a framework through which automated 
regression testing can be done against established baselines as well as support for receipt of live feedback of deployed
pipelines for continuous improvement.

IEvaluate can be extended to support any variety of AI pipelines through the plugin system, although it is specifically 
written with the intention of supporting clinical applications, and in particular clinical information extraction and 
phenotyping tasks.

## Components 
[IEvaluate-Parent](https://www.github.com/integrated-evaluation-framework/IEvaluate-Parent) (You are here) - The parent 
project that contains all components of the framework. Clone this to build the whole stack   

[IEvaluate-API](https://www.github.com/integrated-evaluation-framework/IEvaluate-API) - The API provides a relatively
static point of access for extensions to the IEvaluate Framework, most notably through the use of Plugins to introduce
new integrations and application types. It is recommended that all extension plugins interact as much as possible with
classes from this API as behaviour consistency is guaranteed 

[IEvaluate-Core](https://www.github.com/integrated-evaluation-framework/IEvaluate-Core) - The Integrated Evaluation
Framework's core functionality and several default implementations of the API

[IEvaluate-REST](https://www.github.com/integrated-evaluation-framework/IEvaluate-REST) - Exposes IEvaluate's 
capabilities as a RESTful service

[IEvaluate-Web](https://www.github.com/integrated-evaluation-framework/IEvaluate-Web) - Interacts with the RESTful 
service to provide a front-end to IEvaluate's capabilities

[IEvaluate-ML]() - An IEvaluate Plugin that leverages Elasticsearch's innate ML capabilities to accelerate the debugging
process, as well as utilizing anomaly detection to monitor application errors in a live environment 

[IEvaluate-ClinicalIE-Plugin]() - An example implementation of an IEvaluate plugin that supplies 
