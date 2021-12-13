---
marp: true
theme: default
class: invert
paginate: true
style: |
    img[alt~="center"] {
      display: block;
      margin: 0 auto;
    }
backgroundColor: #fff
backgroundImage: url('https://i2.wp.com/files.123freevectors.com/wp-content/original/110414-black-blurred-background-vector.jpg?w=800&q=95')

---
<!-- _class: lead invert -->
# The Well-Architected Framework
## Build a secure, high-performing, resilient, and efficient cloud infrastructure
### Part II: Operational Excellence & Performance Efficiency

---
## Five+ pillars

![center](https://d2908q01vomqb2.cloudfront.net/77de68daecd823babbb58edb1c8e14d7106e83bb/2020/09/02/Well-Architected-Consulting-1.jpg)


---

## Operational Excellence

&#8594; covers the operations and processes that keep an application running in production

- Deployments must be reliable and predictable
- Automate deployments to reduce the chance of human error. Fast and routine deployment processes won't slow down the release of new features or bug fixes. 
- Quickly roll back or roll forward if an update has problems.

---

## Operational Excellence

### Automation

&#8594; reduce percentage of toil

- ensure consistency
- centralize mistakes
- identify issues quickly
- maximize employee productivity

&#8594; Infrastructure Deployment & Configuration, Operational Tasks

---

## Operational Excellence

1. Optimize build and release processes
2. Monitor system and understand operational health
3. Microservices & DevOps Model
4. Rehearse recovery and practice failure
5. Embrace continuous operational improvement

---

## Operational Excellence: Optimize build and release processes

- Landing zones in place
- Keep environments as similar as possible
- Continuous Integration & Continuous Delivery
    - Integrate tests
- Automated Testing
    - Unit testing
    - Smoke Testing

---

## Operational Excellence: Optimize build and release processes

- Infrastructure as Code
    - Integrate in process: Peer review, automated scanning
    - Avoid configuration drift
    - Easily manage multiple environments
    - Make frequent, small, reversible changes
    - Access control and audit changes
    - Declarative approach toolings: ARM Templates, CloudFormation, Terraform, ...

---

## Operational Excellence: Optimize build and release processes

- Configuration as Code
    - Bootstrap & patch automation
    - Tools:
        - VM extensions, cloud-init, PowerShell Desired State Configuration (DSC), Chef, Puppet

---

## Operational Excellence: Optimize build and release processes

- Event response
    - Use processes for event, incident, and problem management
    - Have a process per alert
    - Prioritize operational events based on business impact
    - Define escalation paths
    - Automate responses to events

---

## Operational Excellence: Monitor system and understand operational health


- Monitor build and release processes
    - Monitor infrastructure and application health
        - Track availability of the system and its components
        - Track application telemetry
        - Track user activity
    - Understand workload health to meet business goals
        - SLAs
        - Compliance

---

## Operational Excellence: Monitor system and understand operational health

&#8594; Monitoring and diagnostics are crucial.

Best practices:
- Correlate application and resource level logs
- Define clear retention times on storage for cold analysis
- Analyze long-term trends analyzed to predict operational issues

---

## Operational Excellence: Monitor system and understand operational health

![width:1000px center](https://docs.microsoft.com/en-us/azure/architecture/best-practices/images/monitoring/pipeline.png)

---

## Operational Excellence: DevOps & Microservices
- Microservices design
    - Independent components
    - Deploy, patch, update systems independently
    - Reduce blast radius
- Strive for a true DevOps Model
    - Create multidisciplinary teams that now work together with shared and efficient practices and tools
    - DevOps model positions the responsibility of operations with developers

---

## Operational Excellence: DevOps & Microservices
### Traditional Model
![width:700px center](https://docs.aws.amazon.com/wellarchitected/latest/operational-excellence-pillar/images/image3.png)

---

## Operational Excellence: DevOps & Microservices
### Separated Application Engineering and Operations (AEO) and Infrastructure Engineering and Operations (IEO)
![width:300px center](https://docs.aws.amazon.com/wellarchitected/latest/operational-excellence-pillar/images/image4.png)

---

## Operational Excellence: DevOps & Microservices
### Separated AEO and IEO with Decentralized Governance
![width:300px center](https://docs.aws.amazon.com/wellarchitected/latest/operational-excellence-pillar/images/image6.png)

---

## Operational Excellence: DevOps & Microservices
Relationship & Owners:
- Resources have identified owners
- Processes and procedures have identified owners
- Team members know what they are responsible for
- Mechanisms exist to identify responsibility and ownership

---

## Operational Excellence: Rehearse recovery and practice failure

- Rehearse recovery
- Practice failure
    - Fault injection
    - Business Continuity Drills
    - *Pre-mortem* exercises
- Use rollbacks of PaaS offerings (or k8s)

---

## Operational Excellence: Embrace continuous operational improvement
- Evolve processes
    - Regular review and validation
    - Share knowledge across teams
    - Post-incident analysis
- Optimizing inefficiencies through automation
    - Operational tasks
    - Rule of three

---

## Performance Efficiency

&#8594; ability of the systzem to adapt to changes

- ability of your workload to scale to meet the demands placed on it by users in an efficient manner

---
 
## Performance Efficiency: Principles

- Understand the challenges of distributed architectures
    - Scaling
        - Design for scaling
        - Scaling issues
        - Scale as a unit
        - Take advantage of platform autoscaling features
        - Improve scalability with session affinity
    - Be aware of antipatterns
        - e.g. *Improper instantiation*, *Noisy Neightbour*, *No Caching*

---
 
## Performance Efficiency: Principles

- Understand the challenges of distributed architectures
    - Build with microservices
    - Asynchronous Request-Reply pattern / Asynchronuous programming
    - Process faster by queuing and batching requests
    - Implement background jobs

---

## Performance Efficiency: Principles

- Go global
- Choose the right service
    - Data storage
    - Correct VM size
    - Use serverless architectures if possible

---

## Performance Efficiency: Principles

- Run performance testing
    - Establish baselines
    - During all stages of the development and deployment life cycle
    - Load and stress testing
    - Shared team responsibility
    - Configure the environment based on testing results to sustain performance efficiency
        - Plan for a load buffer to accommodate random spikes without overloading the infrastructure

---

## Performance Efficiency: Principles

- Continuously monitor the application and the supporting infrastructure
    - Use distributed tracing to build and visualize end-to-end transaction flows for the application.
    - With Scaling in mind
    - Store logs and key metrics of critical components for statistical evaluation and predicting trends.
- Invest in capacity planning
    - Preemptive scaling based on trends
    - Prepare infrastructure for large-scale events
    - Use metrics to fine-tune scaling

---

## Useful Links

- [Operational Excellence Checklist (Azure)](https://docs.microsoft.com/en-us/azure/architecture/checklist/dev-ops)

- [Operational Excellence Patterns (Azure)](https://docs.microsoft.com/en-us/azure/architecture/framework/devops/devops-patterns)

- [Operational Excellence Pillar (AWS)](https://docs.aws.amazon.com/wellarchitected/latest/operational-excellence-pillar/welcome.html)

- [Performance Efficiency Checklist (Azure)](https://docs.microsoft.com/en-us/azure/architecture/framework/scalability/performance-efficiency)

- [Performance Efficiency Patterns (Azure)](https://docs.microsoft.com/en-us/azure/architecture/framework/scalability/performance-efficiency-patterns)

- [Performance Efficiency Pillar (AWS)](https://docs.aws.amazon.com/wellarchitected/latest/performance-efficiency-pillar/welcome.html)
