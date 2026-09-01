Client A – Startup Company

Recommended Platform: Amazon Web Services (AWS)

AWS is a suitable choice for the startup because it provides services that can scale as the company grows. AWS also provides startup programs and resources that can help new companies develop and launch applications. For a mobile application, the startup can use managed and serverless services to reduce the need to manage physical servers. AWS Lambda can automatically scale according to application demand, which can be useful when the number of users increases.

Suggested Services

* **AWS Lambda** – runs application code without requiring the startup to manage servers.
* **Amazon S3** – stores application files, images, backups, and other data.
* **Amazon DynamoDB** – provides a managed NoSQL database suitable for scalable applications.

---

Client B – University

Recommended Platform: Microsoft Azure

Microsoft Azure is the most appropriate choice because the university already uses Windows Server, Microsoft 365, and Active Directory. Azure provides strong integration with Microsoft's identity and enterprise technologies. Microsoft Entra ID can work with Microsoft 365 and can integrate with on-premises Active Directory through synchronization and single sign-on. This can make the migration easier for the university because it can continue using familiar Microsoft technologies while moving selected workloads to the cloud.

Suggested Services

* **Azure Virtual Machines** – hosts Windows Server and other applications.
* **Microsoft Entra ID** – manages identities and access.
* **Azure Blob Storage** – stores documents, images, and backups.

---

Client C – AI Research Company

Recommended Platform: Google Cloud Platform (GCP)

Google Cloud is a strong choice for the AI research company because it provides specialized infrastructure for artificial intelligence and machine learning workloads. Google Cloud offers GPU-enabled Compute Engine resources that can be used for high-performance computing and machine learning. Vertex AI also provides a managed platform for training and deploying machine learning models. These capabilities make Google Cloud suitable for a research organization that requires significant computing power for AI and ML applications.

Suggested Services

* **Google Compute Engine** – provides virtual machines and GPU-enabled computing resources.
* **Vertex AI** – provides tools for developing, training, and deploying machine learning models.
* **Google Kubernetes Engine (GKE)** – runs and manages containerized AI applications.

---

Client D – Global E-Commerce Company

Recommended Platform: Amazon Web Services (AWS)

AWS is a suitable choice for the global e-commerce company because it provides services designed for scalable and highly available applications. The company can distribute its infrastructure across multiple Availability Zones and use load balancing and automatic scaling to handle changes in customer traffic. AWS Lambda can automatically scale according to incoming requests, while other AWS services can provide storage, databases, and networking. This combination can help the company handle traffic increases while maintaining application availability.

### Suggested Services

* **Amazon EC2** – provides scalable virtual servers for application workloads.
* **Elastic Load Balancing (ELB)** – distributes incoming traffic across application resources.
* **Amazon S3** – provides scalable object storage for images, files, and other e-commerce data.
* **Amazon RDS** – provides managed relational database capabilities.

## References

### Amazon Web Services

* AWS. *Getting Started with AWS*. https://aws.amazon.com/aws-startups/learn/how-to-get-started-with-aws/
* AWS. *AWS Lambda*. https://aws.amazon.com/lambda/
* AWS. *AWS Lambda Features*. https://aws.amazon.com/lambda/features/
* AWS. *AWS Startups*. https://aws.amazon.com/startups/

### Microsoft Azure

* Microsoft Learn. *Azure Integration with Microsoft 365*. https://learn.microsoft.com/en-us/microsoft-365/enterprise/azure-integration
* Microsoft Learn. *Microsoft Entra ID*. https://learn.microsoft.com/en-us/entra/

### Google Cloud

* Google Cloud. *Cloud GPUs*. https://cloud.google.com/gpu
* Google Cloud Documentation. *About GPUs on Google Cloud*. https://docs.cloud.google.com/compute/docs/gpus/overview
* Google Cloud. *Vertex AI*. https://cloud.google.com/vertex-ai



# Checkpoint 6 – Multi-Cloud Decision Matrix

| Business Requirement        | Recommended Platform | Justification                                                                                                                                                                                                                                           |
| --------------------------- | -------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Startup Company**         | **AWS**              | AWS provides scalable services that allow a startup to begin with the resources it needs and increase capacity as the application grows. Services such as EC2, S3, and Lambda can support application development and deployment.                       |
| **Enterprise Organization** | **AWS**              | AWS provides a broad range of services for computing, storage, databases, networking, security, and monitoring. Its large service portfolio makes it suitable for organizations with different and complex cloud requirements.                          |
| **Microsoft Environment**   | **Microsoft Azure**  | Azure is the best choice for organizations already using Microsoft technologies. It integrates with Windows Server, Microsoft 365, and Microsoft Entra ID, making it easier to connect existing Microsoft systems with cloud services.                  |
| **AI / Machine Learning**   | **Google Cloud**     | Google Cloud is a strong choice for AI and machine learning because it provides services and infrastructure designed for AI workloads. Vertex AI and GPU-enabled computing can support the development and deployment of machine learning applications. |
| **Kubernetes Deployment**   | **Google Cloud**     | Google Cloud provides Google Kubernetes Engine (GKE), a managed Kubernetes service. GKE can be used to deploy, manage, and scale containerized applications and is a strong option for Kubernetes-based workloads.                                      |
| **Global Web Application**  | **AWS**              | AWS provides global infrastructure, multiple Availability Zones, load balancing, and automatic scaling. These capabilities can help a web application handle changing traffic while improving availability and scalability.                             |

## Summary

The decision matrix shows that there is no single cloud provider that is best for every situation. AWS is a strong general-purpose choice because of its broad services and scalability, Azure is particularly suitable for Microsoft-based organizations, and Google Cloud is especially attractive for AI, machine learning, and Kubernetes workloads. The best cloud platform should therefore be selected according to the organization's technical requirements, existing environment, budget, and future goals.


AWS EC2 Auto Scaling — AWS explains that EC2 Auto Scaling can increase or decrease EC2 capacity based on application demand and can help maintain availability.
Microsoft Azure and Microsoft 365 integration — Microsoft documents that Microsoft 365 uses Microsoft Entra ID and can integrate with on-premises Active Directory.
AWS Global Infrastructure — AWS documents the use of Regions and Availability Zones for highly available architectures.
Google Cloud AI and Kubernetes — Google Cloud documents the use of Vertex AI and GKE for AI/ML workloads and Kubernetes-based deployments.
