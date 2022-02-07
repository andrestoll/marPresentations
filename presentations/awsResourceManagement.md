---
marp: true
theme: gaia
paginate: true
style: |
    section.lead code {
      color: black;
    }
backgroundColor: #fff
backgroundImage: url('data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/2wCEAAkGBw0HBwcHBw0NBwcHBw0HBwcHDQ8IDQcNFREWFhURFRUYHSggGBolGxUTITEhJSk3LjouFx8zODM4Nyg5LisBCgoKDQ0NGg0NFSsZHx0rKysrKysrKysrKysrKysrKysrKysrKysrKysrKysrKysrKysrKysrKysrKysrKysrK//AABEIAMIBAwMBIgACEQEDEQH/xAAXAAEBAQEAAAAAAAAAAAAAAAAAAgEG/8QAFRABAQAAAAAAAAAAAAAAAAAAABH/xAAYAQEBAQEBAAAAAAAAAAAAAAAAAgMBBv/EABURAQEAAAAAAAAAAAAAAAAAAAAR/9oADAMBAAIRAxEAPwDlxg9s8g0YA0YA0YA0YA0YA0YA0YA0YA0YA0YA0YA0YA0YA0YA0YA0YADBx1owBowBowBowBowBowBowBowBowBowBowBowBowBowBowBowdcYMEqaMAaMAaMAaMAaMAaMAaMAaMAaMAaMAaMAaMAaMAaMAaMAaMAYJpU12KE0pSKE0KRQmlKRQmlKRRU0pSKE0pSKE0pSKKmhSKE0KRQmlKRQmlKRQmtpSNpU0pSKE1tKRomlKRVE1pSIGUqauNoylKRoylKRtGUpSNrU0pSKYylKRTGUpSNamlKRoylKRpWUpSNGUpSNKylKRtGUpSNamlKRTGUpSKYylKRoysKRNKilZ1cXSopSkXSopSkXSopSkXSopSkXSopSkXSopSkXSopSkXSopSkXSopSkXSopSkXSopSkXSopSkXSopSkXSopSkXSopSkXRFaUiKVFKzq4ulRSlIulRSlIulRSlIulRSlIulRSlIulRSlIulRSlIulRSlIulRSlIulRSlIulRSlIulRSlIulRSlIulRSlIulRSlIuiKFIilRSs60i6VFKUi6VFKUi6VFKUi6VFKUi6VFKUi6VFKUi6VFKUi6VFKUi6VFKUi6VFKUi6VFKUi6VFKUi6VFKUi6VFKUi6VFKUi6IoUiKVFKzrSLpUUpSLpUUpSLpUUpSLpUUpSLpUUpSLpUUpSLpUUpSLpUUpSLpUUpSLpUUpSLpUUpSLpUUpSLpUUpSLpUUpSLpUUpSLoihSJpUUrOri6VFKUi6VFKUiq2opSkXSopSkXSopSkXWVNKUiqVNKUiq2opSkVW1FKUiq2opSkVSppSkVW1FKUi6VFbSkVSopSkXSopSkVRNaUiKVIiriqVIUiqVLSkbSpCkVSpCkVSpCkVSpaUjaVLSkbSsYUiqVjCkVSpCkVSpaUjaVjCkVSsYUiqVIUiqVIUiqJo5SMGCVNKwBtKwBtKwBtKwBpWANKwBtGANGANKwBtGANKwBtKwBowBpWANowBtYAAA6AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA//9k=')

---
<!-- 
theme: default
color: white
_class: lead
-->
# AWS Resource Management

---
# Terminology
## Resource and Services

- ***Service***: 
Offering and products of AWS, e.g. the resource type.
- ***Resource***: 
Actual entities you create.

Ex: EC2 -> *i-017dd2b6adfda5de6*

---

## Regions and Availability Zones
- ***Region***: 
Physical location to cluster data centers.
Each AWS Region consists of multiple AZs. 
- An ***Availability Zone*** (AZ) 
One or more discrete data centers with redundant power, networking, and connectivity in an AWS Region. 
AZs in an AWS Region are interconnected with high-bandwidth, low-latency networking.

---
<!-- 
_class: lead
-->
## Amazon Ressource Name (ARN)

- uniquely identifies AWS resources

```
    arn:partition:service:region:account-id:resource-id
    arn:partition:service:region:account-id:resource-type/resource-id
    arn:partition:service:region:account-id:resource-type:resource-id
```

---

![bg center:30% 25%](https://upload.wikimedia.org/wikipedia/commons/thumb/9/93/Amazon_Web_Services_Logo.svg/1200px-Amazon_Web_Services_Logo.svg.png)

---

## Resource Management
### Resource Groups
Collection of AWS resources 
- **that are all in the same AWS Region**, and 
- match the criteria specified in the group's query:
  - Tag-based
  - AWS CloudFormation stack-based

Resource groups can be nested.

---

![bg center:30% 25%](https://upload.wikimedia.org/wikipedia/commons/thumb/9/93/Amazon_Web_Services_Logo.svg/1200px-Amazon_Web_Services_Logo.svg.png)

---

## Resource Management
### AWS Config
- tracks the configuration state 
- shows how your resources are related to one another
- specify rules to define the optimal baseline configuration

---

![bg center:30% 25%](https://upload.wikimedia.org/wikipedia/commons/thumb/9/93/Amazon_Web_Services_Logo.svg/1200px-Amazon_Web_Services_Logo.svg.png)
