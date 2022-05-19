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
# Chaos Engineering
## A practical example with Gremlin

--- 

# Motivation

- Reliability
- Outages cost and hurt

'''
The CEO of British Airways recently explained how one failure that stranded tens of thousands of British Airways (BA) passengers in May 2017 cost the company 80 million pounds ($102.19 million USD).
'''

---

# Definition

Chaos Engineering is a disciplined approach to identifying failures before they become outages.

You literally “break things on purpose” to learn how to build more resilient systems.

---

# History / Origin

- 2010: Netflix Eng Tools team created Chaos Monkey.

Chaos Monkey was created in response to Netflix’s move from physical infrastructure to cloud infrastructure provided by Amazon Web Services, and the need to be sure that a loss of an Amazon instance wouldn’t affect the Netflix streaming experience.

“have found that the best defense against major unexpected failures is to fail often. By frequently causing failures, we force our services to be built in a way that is more resilient”

Simian Army

Netflix decided they would create a new role: the Chaos Engineer.

- Added to AWS reliability pilar, FIS



---

# Principles of Chaos Engineering

![bg right:55% 90%](https://res.cloudinary.com/gremlin/image/upload/t_default,f_auto/principles_of_Chaos_Engineering.png)



Experiments are driven by Fallacies of Ditributed Systems:
e.g. “packet-loss attacks” and “latency attacks”


---

# Benefits


- Customer: the increased availability and durability of service means no outages disrupt their day-to-day lives.

- Business: Chaos Engineering can help prevent extremely large losses in revenue and maintenance costs, create happier and more engaged engineers, improve in on-call training for engineering teams, and improve the SEV (incident) Management Program for the entire company.
- Technical: the insights from chaos experiments can mean a reduction in incidents, reduction in on-call burden, increased understanding of system failure modes, improved system design, faster mean time to detection for SEVs, and reduction in repeated SEVs.

---
# How to get started

https://www.gremlin.com/blog/how-to-get-started-with-chaos-engineering/

https://www.gremlin.com/community/tutorials/chaos-engineering-the-history-principles-and-practice/#how-do-you-plan-for-your-first-chaos-experiments

---
# Gameday

---

Links
- https://github.com/Netflix/SimianArmy
- https://netflixtechblog.com/the-netflix-simian-army-16e57fbab116
- https://aws.amazon.com/de/fis/