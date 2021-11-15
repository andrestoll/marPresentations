---
marp: true
theme: gaia
class: invert
paginate: true
backgroundColor: #fff
backgroundImage: url('https://wallpaperaccess.com/full/2276817.jpg')

---
<!-- _class: lead invert -->
# KubeCon & CloudNativeCon 2021

---


## Cloud Native

The CNCF's definition:

*"Cloud-native technologies empower organizations to build and run scalable applications in modern, dynamic environments such as public, private, and hybrid clouds. Containers, service meshes, microservices, immutable infrastructure, and declarative APIs exemplify this approach."*

---

## CNCF

- Help advance container technology and align the tech industry around its evolution
- Stewardship of projects
- Promotion of the underlying technologies
- Serve the community by making the technology accessible and reliable

<!---
Part of the Linuf Foundation
Membership based
Responsible for Certifications & Events
-->

---
<!-- _footer: 'Image source: https://www.cncf.io/' -->
## CNCF Projects

- Graduated
    - e.g. k8s, Prometheus, Helm
- Incubated
    - e.g. argo, gRPC, KubeEdge, ...
- Sandboxed
    - e.g. 

![bg right:55% 90%](https://www.cncf.io/wp-content/uploads/2020/12/CNCF-Annual-Report-2020-graphics-11.svg)

---
<!-- _footer: 'Image source: https://landscape.cncf.io/images/landscape.png' -->
## CNCF Landscape

![bg center:40% 55%](https://landscape.cncf.io/images/landscape.png)

<!---
Technical Oversight Commitee decides about phases
-->

---

## KubeCon & CloudNativeCon 2021 NA

### Key Takeaways

- Pandemic accelerator for cloud adaption
- Growing complexity is a challenge
- Multi cloud
- Edge computing
- Focus on Day 2 operations, operationalization of k8s
    - Observability, governance, security & management

---
<!-- _footer: 'Image source: https://falco.org/' -->
## Falco

k8s threat detection engine

- Parsing Linux system calls from the kernel
- Asserting the stream against a powerful rules engine
- Alerting when a rule is violated


```
- rule: my_programs_opened_file
  desc: track whenever a set of programs opens a file
  condition: proc.name in (my_programs) and (evt.type=open or evt.type=openat)
  output: a tracked program opened a file (user=%user.name command=%proc.cmdline file=%fd.name)
  priority: INFO
```

![bg right:30% 55%](https://raw.githubusercontent.com/falcosecurity/community/master/logo/primary-logo.png)

---
<!-- _footer: 'Image source: https://snyk.io/' -->
## Snyk

Automatically detect vulnerabilities and accelerate fixing throughout your development process

- Coding & CLI
- Code management
- CI/CD
- Production environment

![bg right:40% 55%](https://snyk.io/wp-content/themes/snyk_v2_etyhadar/dist/images/snyk-logo-patch-new.svg)



---
<!-- _footer: 'Image source: https://crossplane.io/' -->
## Crossplane

Enables teams to abstract infrastructure from multiple clouds and expose them on Kubernetes. 

- build multi-cloud apps, using native services
- provision cloud services from k8s app clusters

![bg right:40% 55%](https://cncf-branding.netlify.app/img/projects/crossplane/stacked/color/crossplane-stacked-color.png)

---
## Useful Links



- Landscape:
    - https://landscape.cncf.io/
- Trail Map:
    https://github.com/cncf/trailmap/blob/master/CNCF_TrailMap_latest.pdf
- Charter:
    - https://github.com/cncf/foundation/blob/master/charter.md

