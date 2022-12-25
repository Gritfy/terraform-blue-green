# Terraform Blue Green Deployment

Blue-green deployments and canary tests(rolling deployment) are deployment strategies that are often used by DevOps engineers to release new software gradually, and identify and mitigate the potential blast radius of a failed software release. This allows you to release new software with near-zero downtime.

If you want to learn more about the Blue-Green deployment strategy refer to the below link from RedHat.inc

[https://www.redhat.com/en/topics/devops/what-is-blue-green-deployment](https://www.redhat.com/en/topics/devops/what-is-blue-green-deployment)

On other hand, AWS's [application load balancer](https://docs.aws.amazon.com/elasticloadbalancing/latest/application/introduction.html) (ALB) automatically distributes incoming traffic to the appropriate service at the application layer. ALBs are different from classic load balancers which only route traffic to [EC2](https://aws.amazon.com/ec2/) instances across multiple availability zones. We can define ALB's [listeners](https://docs.aws.amazon.com/elasticloadbalancing/latest/application/load-balancer-listeners.html) (rules) and [target groups](https://docs.aws.amazon.com/elasticloadbalancing/latest/application/load-balancer-target-groups.html) to dynamically route traffic to services. These rules enable us to run canary tests on and incrementally promote the green environment.

Learn how to use Terraform and AWS's Application Load Balancers for canary tests and blue/green deployments. Learn how to add feature flags to your Terraform configuration by using variables and conditionals. 
