# Questions

## Q1: Demographics 

My role in the team/organization is:

- Mainly operations
- Mainly development
- InfoSec
- Site Reliability Engineer
- Release management
- Testing and/or Quality Assurance
- Architect
- Other

## Q2: How do you run your containers on AWS?

The container orchestrator and compute engine of choice. This is what I am already using in prod or plan to use in the future:

- ECS on EC2
- ECS on Fargate
- EKS on EC2
- EKS on Fargate
- DIY Kubernetes (kops, etc.)
- HashiCorp Nomad
- Docker EE

## Q3: Do you use a single source of truth for your repositories?
- YES
- NO

## Q4: Do you consume third party approved images directly from the provider (coredns, aws-alb-ingress-controller, etc)?
- YES
- NO

## Q5: What repository you currently use or plan to use?
- Docker Hub
- JFrog Repository (On Premise)
- JFrog Repository (On AWS)
- ECR
- Other

## Q6: Are you scanning your container images?

Performing static container image scanning, for example, as part of the build pipeline. I'm using:

- Native ECR scanning
- Clair
- Trivy
- Aqua Security
- StackRox
- Sysdig Secure
- Twistlock
- Nope, not scanning images (yet)

## Q7: Are you scanning containers at runtime?

Performing dynamic container scanning, as part of the container orchestrator and/or runtime. I'm using:

- CNCF Falco
- Aqua Security
- NeuVector
- Nope, not scanning containers (yet)

## Q8: How are you managing sensitive data?

Keeping sensitive data, such as passwords and API keys safe at rest. I'm using:

- AWS Secrets Manager
- AWS Parameter Store
- HashiCorp Vault
- DIY encryption
- Nope, not encrypting sensitive data (yet)

## Q9: Are you signing container images?

Signing container images cryptographically. I'm using:

- CNCF Notary
- CNCF TUF-based
- Nope, not signing my images (yet)

## Q10: How are you managing your supply chain?

I'm managing artefacts such as container images along the supply chain using:

- CNCF in-toto
- Grafeas
- Nope, not managing my supply chain (yet)

## Q11: Policy Management

In order to manage and enforce policies (workflow or regulatory wise) I'm using:

- CNCF Open Policy Agent
- Aqua Security
- Custom solution
- Nope, not managing policies (yet)

## Q12: GitOps

In order to strengthen my security posture I'm planning to or are already applying GitOps as a good practice (using tools such as CNCF Flux in case of Kubernetes).

`YES/NO`

## Q13: Are you using Kubernetes?

`YES/NO`

If the answer to this question Q10 is "Yes", the following questions Q11 to Q14 are asked as well.

## Q14: Kubernetes: Network Policies

To enforce Kubernetes Network Policies, I'm using:

- Weave Net
- Calico
- Cilium
- DIY eBPF
- Via a service mesh
- Nope, not using Network Policies

## Q15: Kubernetes: Pod Security Policies

To enforce runtime policies I am using Kubernetes Pod Security Policies: `YES/NO`

## Q16: Kubernetes: User Management

To manage user identities I'm using:

- IAM users/roles
- Active Directory/LDAP
- SSO (OpenID Connect/dex, etc.)

## Q17: Kubernetes: Least Privileges for AWS Services Access

When using AWS services from apps running on Kubernetes, I'm using:

- IAM roles for service accounts
- `kube2iam`
- `kiam`
- I'm assigning the IAM role to the nodes

## Q18: Any other security-related feature of AWS you're using? Any container security tool?

This is a free-form comment, so feel free to share any other tool you're evaluating or already using. For example, Firecracker for multi-tenancy or `audit2rbac` for generating RBAC roles in Kubernetes.
