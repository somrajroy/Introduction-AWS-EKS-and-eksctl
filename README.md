## AWS EKS Introduction <br/><br/>
* Amazon EKS is a managed service that helps make it easier to run Kubernetes. Through EKS, organizations can run Kubernetes without installing and operating a    Kubernetes control plane or worker nodes. EKS drastically simplifies Kubernetes deployment on AWS. <br/>
* EKS scales, manages, and deploys containerized applications. It typically runs in the Amazon public cloud, but can also be deployed on premises. <br/>
* EKS removes much of the time-sink (and headache) by handling various aspects of the infrastructure (auto-upgrades, patching, self-healing etc.). EKS removes development teams biggest time-sinks. <br/>
* AWS EKS consists of two primary components :<br/>
  * Control plane (master node) : AWS takes care of managing everything including scalability and high availability of the control plane <br/>
  * Data plane is where application/workload runs.<br/>
* [What is Amazon EKS](https://docs.aws.amazon.com/eks/latest/userguide/what-is-eks.html)<br/>
* Following diagram illustrates the process of deploying a cluster on EKS - developer(s) instruct EKS to provision a cluster, cloud resources are provisioned in the background, and then connect to the Kubernetes cluster and run workloads.<br/>
 ![image](https://user-images.githubusercontent.com/92582005/202682530-c79b3d47-9cb0-4553-9109-5c726ee35d4b.png) <br/>
* eksctl : It is a 3rd party command line (CLI) tool for working with EKS clusters that automates many individual tasks.
* Eksctl provides the fastest and easiest way to create a new cluster with nodes for Amazon EKS.<br/>
* [Getting started with AWS EKS with eksctl](https://docs.aws.amazon.com/eks/latest/userguide/getting-started-eksctl.html)<br/>
* [Installing or updating eksctl](https://docs.aws.amazon.com/eks/latest/userguide/eksctl.html)<br/>
* Amazon EKS manages the control plane, but how much or little control customer(s) needs to manage the data plane depends on specific requirements. AWS gives three options to manage data plane nodes.<br/>
  * [Unmanaged worker nodes](https://docs.aws.amazon.com/eks/latest/userguide/worker.html)<br/>
  * [EKS Managed Nodegroups](https://docs.aws.amazon.com/eks/latest/userguide/managed-node-groups.html). Amazon EKS provides managed node groups with automated lifecycle management. This lets customer(s) to automatically create, update, or shut down nodes with one operation. EKS uses Amazon’s latest Linux AMIs optimized for use with EKS. <br/>
  * [AWS Fargate](https://docs.aws.amazon.com/eks/latest/userguide/fargate.html) : This fully take care of managing worker nodes. Amazon Fargate, a serverless container service, runs worker nodes & customers need not worry about managing the underlying server infrastructure.<br/>
