# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
    
    Costs:
    Implementing solution in VM will enable service provider deallocate resources (shutdown VM) when not in use, thus helps saving money. An App Service on other hand is associated with App Service Plan. We can create more app services associating with same App Service Plan.
    
    Scalability:
    Both VM & App Service can be scaled vertically & horizontally
    
    Availability:
    Both VM & App Service have high availability. However VMs can be configured to exceed availability than App Service
    
    Workflow:
    Deploying  App Service is easier & faster

- *Choose the appropriate solution (VM or App Service) for deploying the app*
    I prefer using App Service

- *Justify your choice*
    App Service is a PaaS solution that needs developer to just focus on deployinh the code. Here we are developing a content management system which is always expected to be alive. Hence option of shutting down VMs doesn't help. App Service will provide high scalability & availability & deployment can be done in quick time.



### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 
    Here we are developing a very light weight CMS portal. App services have limited cpu & memory. Had my application needed more computing which may require higher configuration than app service provide, I would have gone for VMs.