**"Can you describe a challenging cloud infrastructure project you led?"**

Certainly. One of the most challenging cloud infrastructure projects I led was at **Frame.io (Adobe)**, where we needed to **scale the video encoding and storage platform** to support an increasing volume of **high-resolution media uploads and real-time collaboration** while ensuring **cost efficiency, reliability, and security**.

### **The Challenge:**

* **Scalability & Performance:** As video content grew exponentially, our **AWS-based infrastructure** struggled with **latency issues, unpredictable workloads, and storage inefficiencies**.
* **Cost Optimization:** Given the high storage and compute demands, our AWS costs were **scaling rapidly**, and we needed to optimize spend without sacrificing performance.
* **Security & Compliance:** Operating in a cloud environment meant balancing **performance needs with strict security and compliance requirements (SOC 2, FedRAMP, NIST CSF framework as well as the  TPN - Trusted partner network dicated by the Motion Picture Association and Academy).**

### **My Approach & Solution:**


1. **Architecting a Multi-Tiered Storage Strategy**
   * We **redesigned our S3 storage strategy** to use a **lifecycle policy** that automatically moved less frequently accessed assets to **S3 Infrequent Access and Glacier** while maintaining performance for active workloads.
   * Introduced **deduplication and compression mechanisms** to reduce redundant data storage.
2. **Optimizing Compute & Infrastructure Costs**
   * Moved workloads to **AWS Fargate (serverless containers)** for auto-scaling efficiency.
   * Implemented **Graviton-based EC2 instances** to reduce costs for compute-intensive tasks.
   * Used **Spot Instances with predictive scaling** for non-latency-sensitive jobs, reducing AWS compute spend by \~30%.
3. **Enhancing Reliability & Observability**
   * Deployed **Kubernetes (EKS) for container orchestration**, ensuring auto-scaling and self-healing workloads.
   * Built **a robust observability stack** using **Datadog, Prometheus, and OpenTelemetry**, improving **MTTR (Mean Time to Resolution) by 40%**.
   * Introduced **blue-green deployments and canary releases**, reducing production deployment failures.
4. **Strengthening Security & Compliance**
   * Integrated **IAM best practices** with **least privilege access (zero trust model)** for better security posture.
   * Implemented **AWS Security Hub, GuardDuty, and Config** to continuously monitor for compliance violations.
   * Automated **infrastructure compliance checks** against frameworks like **SOC 2, FedRAMP, and NIST** using **policy-as-code (Terraform Sentinel, AWS Config Rules).**

### **Results & Impact:**

* **Reduced cloud costs by \~35%** through storage optimizations and compute efficiencies.
* **Increased platform reliability**, ensuring **99.99% uptime** while scaling to handle millions of video files.
* **Improved security posture**, ensuring compliance with **SOC 2 and NIST guidelines**.
* **Accelerated deployments**, reducing release rollback incidents by **over 50%**.

This project was a great example of balancing **performance, cost efficiency, and security** while ensuring **seamless user experience at scale.** I'd be happy to dive deeper into any aspect of this that interests you.