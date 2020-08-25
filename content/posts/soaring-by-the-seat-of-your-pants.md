---
author:
  name: "Patrick Abraham"
date: 2019-08-21
linktitle: SOARing by the seat of your pants 
title: SOARing by the seat of your pants
type:
- post
- posts
weight: 10
---

There's a lot of hype with Security Orchestration, Automation and Response (SOAR) and on paper it basically sells itself.  A product that improves Time To Respond (TTR) metrics whilst decreasing FTE count is a CISO's wet dream.  But unfortunately, many orgs find it difficult to realise value with their SOAR products and in a way are ***soaring by the seat of their pants***. 

This blog post provides some (no marketting) recommendations on how you can realise the most value from your SOAR investment. 

----------------
### Building the right team 
Many SOCs will assume that playbooks can wholely be written by SOC analysts, but in my experience, many SOCs will have difficulties scaling this approach as bad software engineering practices and technical debt consume work products.  If I was building a team, I'd be looking for the following skills

* SOC skills.  Not really a shock, but SOC analysts should be involved throughout the playbook development phase and act as an SME.  

* Software Engineering.  These people bring the engineering know-how on building production-ready code.  Involving them early in the project will save headaches down the track by ensuring that the framework to build playbooks is architectually sound and scalable. 

* process improvement/consulting skills - remembering that doing an inefficient process quickly is still inefficient, it may be worth involving a business analyst to undertake some process optimisation and seeking the most "bang for buck" in playbook candidate selection, etc.  

Finding an individual that poses all of the skills can be difficult (see: expensive).  So get creative - perhaps you can partner with the business to borrow some software engineers on a short term basis.  

-------

### WIP - More to come!

## Playbook Selection


## Setting Standards and Guardrails

### Benefits
* Codification of standards is difficult to enforce, and can be time consuming to deploy at scale. Guardrails can be incorporated 
* Applications (developed by third parties or not) may require some guardrails to function better. For instance, the Phantom Splunk App will default any search to real-time. This is problematic for a number of reasons.

## Use-cases
|Use Case|Description|
|------|------|
|Playbook Name Conventions|Enforces strict naming convention of playbooks to differentiate between 'master playbooks' and 'utility playbooks'.
|Action Name Conventions|Enforces strict naming conventions of actions.|
|All Time Search Guardrail|"run query" of Splunk's Phantom App will default to an all-time search unless the SPL contains "@earliest" and "@latest".|

---
[1] - Reference for 