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

- ***Service***: Offering of AWS, e.g. the resource type. Their products
- ***Resource***: Actual entity you create within your account.

Ex: EC2 -> *i-017dd2b6adfda5de6*

---

## Regions and Availability Zones
- ***Region***: physical location around the world where we cluster data centers.
Each AWS Region consists of multiple, isolated, and physically separate AZs within a geographic area. 
- An ***Availability Zone*** (AZ) is one or more discrete data centers with redundant power, networking, and connectivity in an AWS Region. AZs in an AWS Region are interconnected with high-bandwidth, low-latency networking.

---
<!-- 
_class: lead
-->
## Amazon Ressource Name (ARN)

***Amazon Resource Names*** (ARNs) uniquely identify AWS resources. We require an ARN when you need to specify a resource unambiguously across all of AWS, such as in IAM policies, Amazon Relational Database Service (Amazon RDS) tags, and API calls.

    arn:partition:service:region:account-id:resource-id
    arn:partition:service:region:account-id:resource-type/resource-id
    arn:partition:service:region:account-id:resource-type:resource-id

---

![bg center:30% 25%](https://upload.wikimedia.org/wikipedia/commons/thumb/9/93/Amazon_Web_Services_Logo.svg/1200px-Amazon_Web_Services_Logo.svg.png)

---

## Resource Management
### Resource Groups
Collection of AWS resources **that are all in the same AWS Region**, and that match the criteria specified in the group's query:
- Tag-based
- AWS CloudFormation stack-based

Resource groups can be nested; a resource group can contain existing resource groups in the same region.

---

![bg center:30% 25%](https://upload.wikimedia.org/wikipedia/commons/thumb/9/93/Amazon_Web_Services_Logo.svg/1200px-Amazon_Web_Services_Logo.svg.png)

---

## Resource Management
### AWS Config
- tracks the configuration state of your AWS resources at a point in time
- shows how your resources are related to one anotherso that you can see how a change in one resource might impact another
- specify rules to define the optimal baseline configuration for your resources

---

![bg center:30% 25%](https://upload.wikimedia.org/wikipedia/commons/thumb/9/93/Amazon_Web_Services_Logo.svg/1200px-Amazon_Web_Services_Logo.svg.png)
