### SF-Sandboxes
Procedures, Tools, and Processes for Salesforce Sandboxes

MDK - 1/14/19: Initial Entry

The following is original research by Nick Tipoff:

The Dev sandbox, when refreshed, imports only metadata from the production.  No data FROM the sandbox goes to production.  That means the raw data, or records, like leads, contacts, donations/opportunities, etc. will NOT be imported into sandbox upon refresh.  

 

What WILL be imported is metadata.  Examples:  Dashboards, Reports, Email, Layouts, Objects, Custom Objects(like your custom zip), Permission Sets, Profiles, Roles, Triggers, Workflows, Classes, Pages, Flows, Flow Definitions, Approval Processes, Report Type and Assignment Rules.

 

If we want to migrate data from production into a sandbox, you need to use an import tool like Dataloader.

 

This also applies to the Dev Pro.  Dev Pro just has more storage.

 

The partial copy can copy SOME data.


EMAIL QUICK ACTIONS NOT APPEARING IN SANDBOXES!!!

1.  Go to Setup -> DELIVERABILITY (not EMAIL DELIVERABILITY)
2.  From the top pull down, choose ALL EMAILS (not System Emails Only)
 

Only the FULL will copy all data. 

 

We have 30 Dev, 1 Dev Pro, 1 Partial, and no Full.

 

To your earlier reference, yes, it’s easy to transfer all metadata and data from one sandbox to another, like from testing sandbox to a main “staging” one.  This is what the “cloning” feature does.  It transfers everything from one sandbox to another: all metadata and data. 
