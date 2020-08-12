---
author:
  name: "Patrick Abraham"
date: 2020-03-21
linktitle: SOARing by the seat of your pants 
title: SOARing by the seat of your pants
type:
- post
- posts
weight: 10
---

Conceptually, Security Orchestration, Automation and Response (SOAR) is a CISO's wet-dream.  Among things it's often sold as a way of reducing FTE, improving metrics such as TTR and a manner of minimising attrition and/or analyst fatigue.  When done right, this is all true.  But unfortunately, many orgs find it difficult to reach value realisation with SOAR and in a way, are ***soaring by the seat of their pants***.

This blog post details some of my experiences, and recommendations, on how to realise the most value from your SOC.

### The Avengers of Playbook Development
Most organisations will typically throw their SOC Analysts to both lead and operate the Orchestration program.  This is not without issues; orchestration is a multidisciplinary effort and the skillsets required to build a successful playbook are difficult to find (see: expensive) and as such it may be worth partnering with the following roles within your organisation:

* Software Engineers - these people bring the engineering know-how on building production ready code that adheres to common software development best practices.  These practices are crucial for ensuring that your playbooks are sustainable and ultimately lead to less time spent in running costs.  

* Business Analysts - these people ensure that playbook processes are running as efficiently as possible and that the business is maximising it's "bang for buck" in candidate selection, etc. 

Involvement from these groups will pay dividends in terms of time-saved and can be engaged on short one-week stints. 

Note:  Many readers may be dismayed at not having access to the above.  Fear not - I've provided some tips to assist below. 

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