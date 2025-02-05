# Write-up

### Azure Virtual Machine Assesment
Costs: VMs are often cost-effective when it comes to set up of small scale applications. However, they may become expensive while scaling up due to the requirement of additional resources. Ongoing, you have to pay for the compute resources and storage that use which can vary based on the VM size and type (for this project we chose the lower end). 

Scalability: Vertical scaling is quite easy, it can be scaled by simply increasing the size of the VM. Horizontal scaling however, is a bit more difficult, you have to add more VMs which would require setting up and managing load balancers.

Availability: For a high availability, you would need to set up multiple VMs in different zones (and thus all their load balancers) which would add cost and complexity.

Workflow: You would have an overall high level of control. Control over the OS, runtime and applications, which is useful when apps need custom configs. This does mean though that a lot of management would need to be done and upkept to ensure maintenance.


### Azure App Service Assesment
Costs: The app service is often more cost-effective for small/medium apps, especially when choosing a lower pricing plan like we have done. App service is nice also because costs will be predictable and able to be easily monitored over time.

Scalability: Automatic scaling can be chosen which would allow for scaling on demand, without manual intervention. This, again, would just be chosen on a scaling plan that makes the most sense for the apps' needs.

Availability: With app service, there is built in high availability and disaster recovery. Azure manages all of this.

Workflow: Personally the workflow of app service is easier for me because it allows users to focus on the code rather the infrastructure. Azure would handle the OS updates, patches, and really any other infrastructure things that I would feel bogged down otherwise.


### Appropriate Solution
For this case, I think it would be best to use Azure App Service.
I think this for a variety of reasons. I feel that it would allow for the focus to be on developing the application rather than managing the infrasture as well as ensure reliable performance. Of course there is the possibility of over scaling and accidentally choosing too big of a plan, but I think if dilligently setting up the app service this could be avoided. If the app were to exist this small forever, it may be best to choose the VM because then it could be tiny and upkeep would not really be needed. But, I'm pretending like this could be lighly built out.
