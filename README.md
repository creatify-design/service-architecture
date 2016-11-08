![logo](https://github.com/creatify-design/service-architecture/blob/master/logo.png)

# Creatify Service Architecture and Technology Stack
This document contains a description Creatify's service architecture and technology stack. Creatify has bold ambitions, and the technology requirements are equally as ambitious. We first present a service-orientated description of Creatify's technical system. We then focus on individual supporting services in detail and discuss implementations.

# Creatify Service Architecture
A first attempt at a high-level visual representation of Creatify's service architecture is shown below. Each component is referred to as a *manager* with particular responsibilities. The tasks needed to be completed to meet a manager's responsibilities can be performed by and individual, group of individuals, automated system, or combintation.
![architecture](https://github.com/creatify-design/service-architecture/blob/master/ServiceArchitecture.png)

# Creatify Technology Stack
In this section, we discuss each service (and supporting services) in detail. We define the objective of the manager and their responsibilities.

## Account Manager
Responsibilities:
 * Maximise customer retention (through interaction with Client)
 * Push plugin specification to Plugin Manager
 * Push design specification to Design Manager
 * Push deployment proposals to deployment manager
 * Report operational data to Operations Manager

## Design Manager
Responsibilites:
 * Minimise design time (through interaction with Account Manager)
 * Push individual design work to sub-managers
 * Facilitate customisation

### Content Manager
Responsibilites:
 * Autofill content on request (intelligently)
 * Push individual content generation work to sub-managers
 * Facilitate customisation
 
####Copy Manager
Responsibilites:
 * Autofill copy on request (intelligently)
 * Facilitate customisation
 
####Image Manager
Responsibilites:
 * Autofill images on request (intelligently)
 * Facilitate customisation
 
####Icon Manager
Responsibilites:
 * Autofill icons on request (intelligently)
 * Facilitate customisation
 
### Layout Manager
Responsibilites:
 * Supply layout on request (intelligently)
 * Facilitate customisation
 
### Type Manager
Responsibilites:
 * Supply typeface on request (intelligently)
 * Facilitate customisation
 
## Plugin Manager
Responsibilites:
 * Setup plugins on request
 * Delegate plugin work to sub-managers

### Commerce Manager
Responsibilites:
 * Setup e-commerce functionality on request

### Subscription Manager
Responsibilites:
 * Setup subscription functionality on request
 
### Blog Manager
Responsibilites:
 * Setup blogging functionality on request
 
### Widget Manager
Responsibilites:
 * Setup generic widget functionality on request
 
## Deployment Manager
Responsibilites:
 * Manage deployment tasks

## Hosting Manager
Responsibilites:
 * Manage hosting tasks
 * Log interaction data and send to insight manager

## Insights Manager
Responsibilites:
 * Analyse user data
 * Generate interpretable reports for client
 * Propose product experiments to Account Manager 
 
## Operations Manager
Repsonsibilities:
 * Aggregate operational data from Account Managers
 * Generate operations reports to executives
