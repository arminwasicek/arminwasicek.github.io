---
title: MODESEC Project 
date: 2015-08-01
description: Models and security in Cyber-Physical Systems.
categories:
  - project
  - security
  - cyber-phiscal systems
image:
author_staff_member: armin
---


The objective of the MODESEC project is to research the interaction between modelling and security in the context of Cyber-Physical Systems. The first step towards this goal is to develop and implement a development method for secure cyber physical systems. Our innovation is to investigate on how to use models to gain insights about a system’s security.

* Develop a method for the secure model-based design of a CPS
* Integrate the methodology in a model-based design tool
* Evaluate the Secure Design Methodology in a case study

The proposed approach strives to support CPS engineers that were not trained in cyber security to implement security. This will be achieved by integrating the secure design of a CPS in the model-based design approach to design a CPS. Model-based design tools are familiar to engineers working in many different domains. Thus, our approach enables these engineers to build more secure products by lowering the entry barriers to implement cyber security mechanisms.

## System models and attack models

Designing and implementing appropriate control laws is one of the major tasks when building a CPS. A CPS encompasses sensors and actuators that interface with the physical environment. The control law formulates the way inputs from the sensors are interpreted and how and when outputs to the actuators are made according to the purpose of the system. A system model encompasses models for the controller implementing a control law and the environment the controller operates in. It is standard engineering practice to use system models to explore the design space before actually building a CPS. The system model is the starting point for our secure development method. Our unique approach combines system and attack models, thus, forming a model of a system under attack.

![Alt text](/images/systemattackmodel.svg)

**_Figure 1: Combining System and attack models forms a system under attack_**

An attack model captures potential malicious behavior. Securing a CPS ultimately deals with protecting the CPS' interaction with the physical environment. Therefore, a CPS attack model is not only relevant for the cyber part of the CPS, but also for the physical interface of the CPS. This connection is a unique challenge and separates this research from other efforts on purely software-based computer systems. The MODESEC project investigates how attack models and system models can be combined in a meaningful manner to provide insights on the consequences of attacks in the physical domain.

## Security architecture

The baseline for our solution is a security architecture that encompasses preventive and reactive security mechanisms. Preventive mechanisms actively prohibit a malicious user from accessing or tempering a service, for example, firewalls, access controls, or cryptographic protocols. Reactive mechanisms target recognizing malicious activities in the system. These activities can be known a priori and be specified in a rule set or discovered during the runtime of the system. The secure model-based design method connects to both kinds of mechanisms. For instance, the designer augment modify the system with preventive mechanism such that a given attack model fails as a consequence of the modification. Or the attack model could be transformed in a specification for a reactive mechanism, thus, able to detect certain attacks.

## Work performed

So far, the work has been dedicated to develop a secure design method and a reactive mechanism. First, it was important to learn and understand the methods and tools that a control engineer uses. Second, the concept of aspect-oriented modelling was adapted modelling the security of a system. All artifacts that constitute the secure design method have been implemented and its evaluation has been facilitated. Exemplary attack models have been implemented. A workflow that meets the work habits of control engineers has been specified. Third, an effort was made to develop principles for detecting modifications in the context of automotive systems. A novel intrusion detection approach has been developed and implemented. Finally, a significant amount of time has been dedicated to present the method at conferences, and workshops. Experts have been consulted and companies have been visited.

## Main results

The first main result has been the specification of a secure design method leveraging the concept of aspect-oriented modelling. Aspect-oriented modelling enables a designer to simulate system models and attack models at the same time and in the same modelling environment (Ptolemy II in our case). 

The second main result is the development of a reactive security mechanism that monitors a system’s environment and infers, if the controller has been modified. Both results have been applied to automotive case studies.

## Final results and their potential impact

The goal of this research effort is a modelling approach to analyze and secure control systems with respect to security. We strive to derive a method that enables an engineer to prototype and compare different implementations within a model-based design method such that the engineer gets insights on the trade-offs for increasing the security. The final result will be a secure design method for design space exploration. It will facilitate the implementation of reactive security mechanisms particularly for the physical part of a CPS. Thus, we show how the use of models can contribute to build secure CPS. Application on automotive systems will enhance the visibility of the research, as security concerns in vehicles are currently a topic of high interest. We hope to impact the secure development of novel safety features in the design of the new generation of semi-autonomous and autonomous vehicles.