### Introduction : Managed Kubernetes, AWS EKS & eksctl <br/><br/>
* [Amazon EKS](https://aws.amazon.com/eks/) is a fully managed kubernetes service that helps make it easier to run Kubernetes. Through EKS, organizations can run Kubernetes without installing and operating a Kubernetes control plane or worker nodes. EKS drastically simplifies Kubernetes deployment on AWS.It reduces the complexity of container deployment and management and provides automation. <br/>
* EKS is  is a fully managed, cloud-based service to build, secure and maintain Kubernetes with AWS. It runs, deploys and operate Kubernetes clusters. <br/>
* EKS scales, manages, and deploys containerized applications. It typically runs in the Amazon public cloud, but can also be deployed on premises. <br/>
* EKS removes much of the time-sink (and headache) by handling various aspects of the infrastructure (auto-upgrades, patching, self-healing etc.). AWS handles all the management tasks for the Kubernetes control plane. This includes all security configurations, upgrades and patches. Because it is an Amazon service, EKS integrates with Elastic Load Balancing, AWS Identity and Access Management, AWS CloudTrail and Amazon Virtual Private Cloud. <br/>
* Infrastructure management is smooth; AWS EKS elastically provisions resources, so customers/developers don’t need to worry about whether they’re being used effectively. <br/>
* In addition to Amazon services, admins can move pods to non-AWS environments without application code changes. Thus it helps to create a cloud agnostic/hybrid enviornment easily<br/>
* AWS EKS consists of two primary components :<br/>
  * Control plane (master node) : AWS takes care of managing everything including scalability and high availability of the control plane <br/>
  * Data plane is where application/workload runs.<br/>
  ![image](https://user-images.githubusercontent.com/92582005/202979144-c03581c9-6c50-4975-9f8f-40d1788daac4.png) <br/>
* Following diagram illustrates the process of deploying a cluster on EKS - developer(s) instruct EKS to provision a cluster, cloud resources are provisioned in the background, and then connect to the Kubernetes cluster and run workloads.<br/>
 ![image](https://user-images.githubusercontent.com/92582005/202682530-c79b3d47-9cb0-4553-9109-5c726ee35d4b.png) <br/>
* eksctl : It is a 3rd party command line (CLI) tool for working with EKS clusters that automates individual tasks.<br/>
* Eksctl provides the fastest and easiest way to create a new cluster in Amazon EKS.<br/>
* [Getting started with AWS EKS with eksctl](https://docs.aws.amazon.com/eks/latest/userguide/getting-started-eksctl.html)<br/>
* [Installing or updating eksctl](https://docs.aws.amazon.com/eks/latest/userguide/eksctl.html)<br/>
* [Amazon EKS features](https://aws.amazon.com/eks/features/)<br/>
* [Amazon EKS pricing](https://aws.amazon.com/eks/pricing/) : AWS EKS costs $0.10 per hour (73.00 USD monthly) per cluster (us-west-2) for the master node (control plane). Additional charges will apply as customrs need to pay for the AWS resources necessary to run Kubernetes worker nodes (EC2, LB etc.)<br/>
* Amazon EKS manages the control plane, but how much or little control customer(s) needs to manage the data plane depends on specific requirements. AWS gives three options to manage data plane nodes.<br/>
  * [Unmanaged worker nodes](https://docs.aws.amazon.com/eks/latest/userguide/worker.html)<br/>
  * [EKS Managed Nodegroups](https://docs.aws.amazon.com/eks/latest/userguide/managed-node-groups.html). Amazon EKS provides managed node groups with automated lifecycle management. This lets customer(s) to automatically create, update, or shut down nodes with one operation. EKS uses Amazon’s latest Linux AMIs optimized for use with EKS. <br/>
  * [AWS Fargate](https://docs.aws.amazon.com/eks/latest/userguide/fargate.html) : This fully take care of managing worker nodes. Amazon Fargate, a serverless container service, runs worker nodes & customers need not worry about managing the underlying server infrastructure.<br/><br/>
#### Further references <br/>
* [What is Amazon EKS?](https://docs.aws.amazon.com/eks/latest/userguide/what-is-eks.html)<br/>
* [eksctl - The official CLI for Amazon EKS](https://eksctl.io/) <br/>
* [AWS Command Line Interface (AWS CLI): A Complete Guide](https://neal-davis.medium.com/aws-command-line-interface-aws-cli-a-complete-guide-5897d7f95d5d)<br/>

