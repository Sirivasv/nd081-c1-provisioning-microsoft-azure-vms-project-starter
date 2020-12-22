# Write-up Template 


## Analyze, choose, and justify the appropriate resource option for deploying the app. 

*For **both** a VM or App Service solution for the CMS app:* 

- *Analyze costs, scalability, availability, and workflow* 

- *Choose the appropriate solution (VM or App Service) for deploying the app* 

- *Justify your choice* 

### Costs 

- A hosted VM of standard tier with 1vcore 3gb of ram and 50gb of storage costs around $51.15 per month. 

- An app service with standard tier with 1 vcore, 1.75gb of ram and 50gb of storage costs $69.35 per month. 

### Scalability 

- Both solutions offer an easy option to scale one instance, that is the vertical scaling or scale up, this is because in both services can be easily upgraded by choosing an instance with more CPU, RAM or storage in a slightly similar cost rate, being the app service more expensive than the VM solution. 

- A difference is on the number of instances that can run the application, the horizontal scaling or scale out, while its possible to do it in both solutions in the app service is much easier as it is deployed automatically and can be managed with much ease that with independent VMs manually organized. Still in costs the App service is more expensive. 

### Workflow 

- With the VMs the deployment and developing pipelines must be set by the user, the workflow should be automated and managed by the user, having the control over how many and which type of machines are running the app and independently troubleshooting each of them. This could add up time and efforts worth putting in the app. Also, as all of the used services in the app are Azure products as well, we will be creating the same workflow that is managed automatically by App service. 

- With App Service the workflow is in part managed in the azure portal being automated with the deployments for example, is a much easier experience with the used services being Azure products as well, this allows us to have all the control and troubleshooting in one place. 
 

### Choose a Solution 

- App Service 

### Justify your choice 

- The App Service solution has a major inconvenience that is its cost but it is heavily compensated by the benefits it provides to our current app. Our App can now be not only easily scaled up but scaled out, something that would require more effort with VMs, the workflow could be easily automated within azure allowing us to update and deploy new features in a more consistent and manageable pace across all of our instances, this would be much harder with VMs. And lastly as our used services are also offered by Azure, we can connect to them, log them and troubleshooting in the Azure portal with more support options than with VMs. 

So, if we can afford it, it would be greatly beneficial to use App service, it could even save us money in the future with less errors in our workflow. 

## Assess app changes that would change your decision. 

*Detail how the app and any other needs would have to change for you to change your decision in the last section.*  

- I would say that the major changes in our app that can heavily impact the decision are our used services, actual service demand and budget. First with the budget if we cannot simply afford it then the cheapest option should be the one to go that is VMs, but even if we can afford for App service the following will still make us to choose VMs. 

- Our actual demand, if we are just fine with one instance and we are not expecting a need for a scale out solution, the VMs are as well fitted for this as the App service being even cheaper to upgrade (only vertically). 

- Finally, with the used services, if our stack uses technologies that are not offered by azure using App Service might even being prejudicial as it can hid our specific configuration needs in order to work with our own workflow. 
