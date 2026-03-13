# Deployment Write-Up

## Analyze, Choose, and Justify the Appropriate Resource Option for Deploying the App

For this project, I analyzed both Azure Virtual Machines (VMs) and Azure App Service as possible deployment options for the Flask CMS application. The comparison was based on cost, scalability, availability, and development workflow.

From a **cost perspective**, Azure App Service is generally more affordable than running a full virtual machine. A VM requires paying for the compute instance, storage, and potentially additional networking resources. App Service provides a managed platform that reduces infrastructure costs for smaller web applications like this CMS.

In terms of **maintenance**, a VM requires significant management effort. This includes installing and configuring the operating system, setting up the web server, applying security patches, and maintaining updates over time. Azure App Service is a Platform-as-a-Service (PaaS) offering, which means Azure manages the operating system, security patches, and runtime environment automatically. This significantly reduces operational overhead.

The **development workflow** is also much simpler with Azure App Service. By connecting the App Service to a GitHub repository, the application can be deployed automatically whenever changes are pushed to the repository. This continuous deployment workflow allows faster updates and easier management compared to manually configuring deployment on a VM.

Regarding **availability and reliability**, Azure App Service provides built-in features such as automatic restarts, load balancing, and platform monitoring. While similar reliability can be achieved with a VM, it requires additional manual configuration and management.

For **scalability**, Azure App Service allows easy scaling through the Azure portal by adjusting the pricing tier or scaling instances. For a relatively small application like this CMS, the App Service scaling model is sufficient and easier to manage than configuring scaling manually with virtual machines.

Based on these factors—cost efficiency, reduced maintenance, simplified workflow, built-in availability features, and easy scalability—I chose **Azure App Service** as the deployment solution for this project.

---

## Assess App Changes That Would Change the Decision

Although Azure App Service was the best choice for this project, there are scenarios where using a virtual machine might become more appropriate.

If the application required **full control over the operating system or server configuration**, a VM would provide greater flexibility. For example, applications that require custom system-level software, specialized networking configurations, or unsupported runtimes may require deployment on a virtual machine.

Additionally, if the application were significantly more complex—such as requiring multiple services, custom infrastructure setups, or specialized security configurations—a VM-based architecture might provide greater customization.

However, for a relatively straightforward web application like this Flask CMS, Azure App Service provides a simpler, more efficient, and more maintainable deployment solution.
<img width="1918" height="876" alt="image" src="https://github.com/user-attachments/assets/491840de-0dbe-4cef-82c9-8dfe2b06414c" />
