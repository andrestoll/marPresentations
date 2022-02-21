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
    a {
        color: red;
    }
backgroundColor: #fff
color: #645dd7

---
<!-- _class: lead invert -->
# Fallacies of Distributed Systems
## Build a secure, high-performing, resilient, and efficient cloud infrastructure

---

The 8 fallacies should serve as a warning for architects and designers of distributed systems.

Believing these statements are true results in troubles and pains for the system and its creators further down the line. 

We should expect and prepare for the exact opposite of these statements if we want to have a dependable distributed system.

---

## The Network Is Reliable

Problem:
- Calls over a network will fail

Solutions:
- Fault tolerant infrastructure
- Automatic retries
- Idempotency and Determinism


![bg right:45% 90%](https://www.mycertnotes.com/wp-content/uploads/2020/08/Figure-9-2.-The-network-is-not-reliable.png)

---

## Latency Is Zero
Problem:
- Calls over a network are not instant

Solutions:
- Bring back all the data you might need
- Move the data closer to the clients

![bg right:45% 90%](https://www.mycertnotes.com/wp-content/uploads/2020/08/Figure-9-3.-Latency-is-not-zero.png)

---

## Bandwidth Is Infinite

Problem:
- Bandwidth is limited

Solutions:
- Network traffic control
- Lightweight data formats

![bg right:45% 90%](https://www.mycertnotes.com/wp-content/uploads/2020/08/Figure-9-4.-Bandwidth-is-not-infinite.png)

---

## The Network Is Secure

Problem:
- The network is insecure

Solutions:
- Defense in Depth
- Security mindset
- Threat modelling

![bg right:45% 90%](https://www.mycertnotes.com/wp-content/uploads/2020/08/Figure-9-5.-The-network-is-not-secure.png)

---

## Topology Doesn't Change

Problem:
- The topology ***does*** change constantly

Solutions:
- Abstract the physical structure of the network
- Cattle, not pets
- Test (Chaos Engineering)

![bg right:45% 90%](https://www.mycertnotes.com/wp-content/uploads/2020/08/Figure-9-6.-The-network-topology-always-changes.png)

---

## There is One Administrator

Problem:
- There is no one person that knows everything

Solutions:
- Embrace DevOps
- Centralized Logging & Monitoring

![bg right:45% 90%](https://www.mycertnotes.com/wp-content/uploads/2020/08/Figure-9-7.-There-are-many-network-administrators-not-just-one.png)

---

## Transport Cost Is Zero

Problem:
- Transport cost is not zero

Solutions:
- Efficiency

![bg right:45% 90%](https://www.mycertnotes.com/wp-content/uploads/2020/08/Figure-9-8.-Remote-access-costs-money.png)

---

## The Network Is Homogeneous

Problem:
- The network is heterogenous

Solutions:
- Choose standard formats

![bg right:45% 90%](https://www.mycertnotes.com/wp-content/uploads/2020/08/Figure-9-9.-The-network-is-not-homogeneous.png)
