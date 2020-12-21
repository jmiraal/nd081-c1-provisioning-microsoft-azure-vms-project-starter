# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

We have opted by deploying an App Service instead of a Virtul Machine due to the next reasons:

* The project is very simple and the App Service option is the easiest and cheaper way of implementing a web app. In general, the App Service has a lower cost.
* The nature of the app fits perfectly in the use cases that the App Service was designed for. It is a light weight web app. It is not very demanding with the resources that are needed in its basci design.
* We can achieve a high availability in both cases. Besides that, a Virtual Machine can be switched down when it is not used to reduce costs, but this service is expected to be running all the time, so this possible advantage makes no sense in our case.
* We don't need aslo many of the advantages of a Virtual Machine, since it is unnecessary to control the OS, the app is developed in Python, which is perfectly suported by the App Service, and we don't need to install any additional software.
* We don't have information about the theoretical use of the app. If it is thinked for beeing used inside an organization, a company or a school, the number of possible users will be limited and the resource requirements will not probably exceed the limit of the Service.


### Assess app changes that would change your decision.

* We can monitorize the use of the application and the resources consumed. We have a wide margin to increase its capacity. The app is quite light and it doesnt't use many CPU, but if we store a lot of posts, we could need more than the maximum 14Gb available. This can occur also if we make a change allowing the users to add many photos per post. We could implement a modification to limit the size of each photo also.
* We may need also to migrate to VM if the company impose to us some restrictions in terms of SO configuration or if we are thinking about migrating the platform to other vendor in the future.
* Anyway, if we were close to the limit of maximum capacity for the App Service, it wouldn't be difficult to migrate to a Virtual Machine.
