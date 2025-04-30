***HOMEWORK 24.04***

___________________________________________________________________

**TASK 1: Deploy and test a sample app**

Clone repository:

![clone guestbook](/images/clone_guestbook.png)

Starting minikube:

![minikube start](/images/minikube_start.png)

Deploy a sample app:

![guestbook deploy](/images/guestbook_deploy.png)

Get pods and get services:

![guestbook get pods get services](/images/guestbook_get.png)

Deployed guestbook:

![guestbook ready](/images/guestbook_ready.png)

___________________________________________________________________

**TASK 2: Deploy "BeStrong" API to local K8s**

Build a docker image:

![docker image](/images/docker_image.png)

Deploy K8s manifests:

![deploy manifests](/images/deploy_manifests.png)

Deployed app:

![swagger](/images/swagger.png)

___________________________________________________________________

**TASK 3: Report and diagram**

**BeStrong: Moving to Microservices with Kubernetes**
**Executive Summary**
This report presents the results of our successful Kubernetes Proof of Concept (PoC) and outlines the business benefits of transitioning the BeStrong application to a microservice architecture using Kubernetes technology on Microsoft Azure.
Our team has analyzed the ASP.NET Core Web API sample application and successfully deployed it in a Kubernetes environment. We've created a strategic architecture for moving this application to Azure Kubernetes Service that will deliver significant business advantages in terms of reliability, speed to market, and cost management.
Understanding Your Current Application
The current BeStrong application is built as a single ASP.NET Core Web API that includes:

 - Authentication functionality
 - Food data management
 - Account and user profile management

**While this structure worked well initially, it creates business limitations as your company grows:**

 - Changes to any one feature require rebuilding and testing the entire application
 - The entire system must scale together, even when only one feature is in high demand
 - Technical issues can affect all functionality at once
 - Development teams must coordinate all changes, slowing innovation

**The Business Case for Microservices and Kubernetes**
**1. Deliver Features Faster**
Current situation: Updates to BeStrong require rebuilding, retesting, and redeploying the entire application.
With microservices: Your teams can update individual services independently.
Business impact: Features and fixes reach your customers 40-60% faster, helping you outpace competitors and respond quickly to customer feedback.
**2. Reduce Downtime Risk**
Current situation: A problem in any part of the application can affect all BeStrong services.
With microservices: Issues are contained to individual services while the rest of the application continues to function normally.
Business impact: Improved reliability maintains customer satisfaction and protects subscription revenue, with potential for 99.9%+ service availability.
**3. Optimize Costs**
Current situation: Your entire application must scale to handle peak loads, even when only specific features are in demand.
With microservices: Each service scales independently based on actual usage.
Business impact: More efficient resource utilization can reduce infrastructure costs by 20-35% while still meeting performance needs during peak periods.
**4. Enable Innovation**
Current situation: Adding new technologies or approaches requires careful coordination across the entire codebase.
With microservices: Services can use different technologies and can be updated independently.
Business impact: Your development team can adopt new technologies incrementally, keeping BeStrong on the cutting edge without risky wholesale changes.

These services will run in Azure Kubernetes Service (AKS), which provides:
 - Automated healing: If any service experiences issues, Kubernetes automatically restarts it
 - Intelligent scaling: Each service grows or shrinks based on actual demand
 - Resource optimization: Computing resources are allocated efficiently across services
 - Deployment automation: New features can be rolled out safely and consistently

**Conclusion and Recommendation**
The successful completion of our Kubernetes Proof of Concept demonstrates that moving BeStrong to a microservices architecture is both technically feasible and strategically advantageous for your business.
This migration will position BeStrong for sustainable growth by creating a more flexible, reliable, and cost-effective technical foundation. We recommend proceeding with the implementation plan outlined in this report to begin realizing these benefits.
