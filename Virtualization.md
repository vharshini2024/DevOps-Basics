**1. What is virtualization really?**

> Virtualization is the process of using one physical server to run multiple virtual machines (VMs) using a software called Hypervisor.

**2. So what is this Hypervisor, exactly?**

> It’s just a software that allows multiple VMs to share the same physical hardware.  
> Hypervisor is not some magical cloud thing. It's a real installable software — just like you install Zoom or Chrome, someone installs this on the physical server.

**3. Who installs the Hypervisor?**

Let’s split this into two scenarios:

**A. In a normal data center (on-prem):**

- There's a team called Infra Engineers / SysAdmins.
- They are the ones who physically install the hypervisor (like VMware ESXi) on bare metal servers.
- After installation, they give access to DevOps or Platform teams to create and manage VMs.
- You, as a DevOps engineer, may not install the hypervisor, but you will:
  - Create VMs
  - Deploy tools
  - Automate provisioning
  - Integrate monitoring/logging/CI-CD over these VMs

**B. In a cloud environment (Azure/AWS/GCP):**

- Cloud providers like Azure already install and manage the hypervisors behind the scenes.
- When you create a VM in Azure, you're not touching the hypervisor — you’re just using their interface (portal/CLI/Terraform) to ask for a VM.
- So here, virtualization is happening under the hood, but you're not managing the hypervisor — just leveraging it.

**Simple terms:**

- Virtualization = Running multiple VMs on one physical machine.
- Hypervisor = Software that makes this possible.

**Who installs it?**

- On-prem: Infra guys.
- Cloud: Azure/AWS/GCP already handle it.

**We as DevOps?**

- You use VMs, automate them, deploy to them — but don’t usually install hypervisors.
