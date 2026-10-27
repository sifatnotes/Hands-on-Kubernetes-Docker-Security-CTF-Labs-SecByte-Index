# Hands-on-Kubernetes-Docker-Security-CTF-Labs-SecByte-Index
A complete catalog of practical cybersecurity CTF labs covering Kubernetes cluster security, container escapes, privilege escalation, Pod security, network policies, Docker forensics, incident response, and secrets management.
# Kubernetes & Docker Container Security CTF Lab Collection

Welcome to the **Kubernetes & Docker Container Security CTF Lab Collection**. This repository serves as a practical, searchable index of hands-on security labs and Capture The Flag (CTF) challenges hosted on Learn SecByte.

This collection focuses on cloud-native container security, covering Kubernetes cluster architecture, container breakout techniques, cluster privilege escalation, NetworkPolicy isolation, Docker digital forensics, container incident response, and secrets protection.

---

## Lab Collection Index

### 1. Kubernetes Architecture, Hardening & Attack Surface
* **Kubernetes Architecture: Control Plane & Pod Security**  
  *Lab Link:* [https://learn.secbyte.org/ctf/kubernetes-architecture-control-plane-pod-security](https://learn.secbyte.org/ctf/kubernetes-architecture-control-plane-pod-security)  
  *Focus:* Control plane component isolation (kube-apiserver, etcd, controller-manager, scheduler), Pod Security Standards (PSS), and admission controllers.

* **Kubernetes Hardening Fundamentals**  
  *Lab Link:* [https://learn.secbyte.org/ctf/kubernetes-hardening-fundamentals](https://learn.secbyte.org/ctf/kubernetes-hardening-fundamentals)  
  *Focus:* Applying CIS Kubernetes Benchmarks, disabling anonymous authentication, restricting API server endpoints, and enforcing rootless execution.

* **Kubernetes Attack Surface: Misconfigurations to Cluster Takeover**  
  *Lab Link:* [https://learn.secbyte.org/ctf/kubernetes-attack-surface-misconfigurations-cluster-takeover](https://learn.secbyte.org/ctf/kubernetes-attack-surface-misconfigurations-cluster-takeover)  
  *Focus:* Identifying exposed kubelet ports, open dashboard interfaces, permissive service accounts, and misconfigured RBAC roles.

* **Kubernetes Services: Exposing Workloads Safely**  
  *Lab Link:* [https://learn.secbyte.org/ctf/kubernetes-services-exposing-workloads-safely](https://learn.secbyte.org/ctf/kubernetes-services-exposing-workloads-safely)  
  *Focus:* Securing NodePort, LoadBalancer, and Ingress routing, TLS termination, and mitigating unauthorized workload exposure.

* **Kubernetes Network Policies: Contain the Pod-to-Pod Blast Radius**  
  *Lab Link:* [https://learn.secbyte.org/ctf/kubernetes-network-policies-contain-the-pod-to-pod-blast-rad](https://learn.secbyte.org/ctf/kubernetes-network-policies-contain-the-pod-to-pod-blast-rad)  
  *Focus:* Authoring CNI-enforced NetworkPolicies, default-deny ingress/egress boundaries, and micro-segmenting namespace traffic.

* **Kubernetes Secrets: Finding, Understanding, and Defending Sensitive Data**  
  *Lab Link:* [https://learn.secbyte.org/ctf/kubernetes-secrets-finding-understanding-and-defending-sensi](https://learn.secbyte.org/ctf/kubernetes-secrets-finding-understanding-and-defending-sensi)  
  *Focus:* Auditing base64 secret storage, enabling envelope encryption at rest with KMS, RBAC access controls, and secret mounting risks.

### 2. Kubernetes Exploitation & Container Breakout
* **Kubernetes Container Escape: From Pod Breakout to Node Compromise**  
  *Lab Link:* [https://learn.secbyte.org/ctf/kubernetes-container-escape-from-pod-breakout-to-node-compro](https://learn.secbyte.org/ctf/kubernetes-container-escape-from-pod-breakout-to-node-compro)  
  *Focus:* Exploiting mounted host sockets (`docker.sock`, `containerd.sock`), privileged containers, kernel vulnerabilities, and host filesystem escapes.

* **Kubernetes Privilege Escalation: From Pod Access to Cluster Compromise**  
  *Lab Link:* [https://learn.secbyte.org/ctf/kubernetes-privilege-escalation-from-pod-access-to-cluster-c](https://learn.secbyte.org/ctf/kubernetes-privilege-escalation-from-pod-access-to-cluster-c)  
  *Focus:* Leveraging default service account tokens, over-privileged ClusterRoles, impersonation rights, and lateral movement across namespaces.

### 3. Docker Security, Forensics & Incident Response
* **Docker Compose Security**  
  *Lab Link:* [https://learn.secbyte.org/ctf/docker-compose-security](https://learn.secbyte.org/ctf/docker-compose-security)  
  *Focus:* Auditing multi-container orchestration configs, bridge network isolation, capability drops (`cap_drop`), and environment variable leaks.

* **Docker Secrets: Securely Managing Sensitive Data in Containers**  
  *Lab Link:* [https://learn.secbyte.org/ctf/docker-secrets-securely-managing-sensitive-data-in-container](https://learn.secbyte.org/ctf/docker-secrets-securely-managing-sensitive-data-in-container)  
  *Focus:* Eliminating hardcoded credentials in Dockerfiles, leveraging Swarm/Compose secrets, and secure runtime volume mounting.

* **Docker Forensics: Investigating Containerized Intrusions**  
  *Lab Link:* [https://learn.secbyte.org/ctf/docker-forensics-investigating-containerized-intrusions](https://learn.secbyte.org/ctf/docker-forensics-investigating-containerized-intrusions)  
  *Focus:* Analyzing container layer diffs, acquiring overlay2 artifacts, container memory dumps, and inspecting daemon log streams.

* **Docker Incident Response: Investigate, Contain, Eradicate**  
  *Lab Link:* [https://learn.secbyte.org/ctf/docker-incident-response-investigate-contain-eradicate](https://learn.secbyte.org/ctf/docker-incident-response-investigate-contain-eradicate)  
  *Focus:* Isolating compromised containers, committing state snapshots for triage, pausing execution, and removing persistent backdoors.

---

## Learning Path

### Path A: Kubernetes Cluster Hardening & Defense
1. **Architecture & Standards:** Start with [Kubernetes Architecture: Control Plane & Pod Security](https://learn.secbyte.org/ctf/kubernetes-architecture-control-plane-pod-security) and [Kubernetes Hardening Fundamentals](https://learn.secbyte.org/ctf/kubernetes-hardening-fundamentals).
2. **Access Control & Network Boundary:** Implement controls via [Kubernetes Network Policies](https://learn.secbyte.org/ctf/kubernetes-network-policies-contain-the-pod-to-pod-blast-rad), [Kubernetes Services](https://learn.secbyte.org/ctf/kubernetes-services-exposing-workloads-safely), and [Kubernetes Secrets](https://learn.secbyte.org/ctf/kubernetes-secrets-finding-understanding-and-defending-sensi).
3. **Attack Surface Auditing:** Analyze vulnerabilities using [Kubernetes Attack Surface: Misconfigurations to Cluster Takeover](https://learn.secbyte.org/ctf/kubernetes-attack-surface-misconfigurations-cluster-takeover).

### Path B: Container Breakout & Offensive Security
1. **Misconfiguration Exploitation:** Practice with [Kubernetes Attack Surface](https://learn.secbyte.org/ctf/kubernetes-attack-surface-misconfigurations-cluster-takeover).
2. **Escape & Escalation:** Execute advanced tactics in [Kubernetes Container Escape](https://learn.secbyte.org/ctf/kubernetes-container-escape-from-pod-breakout-to-node-compro) and [Kubernetes Privilege Escalation](https://learn.secbyte.org/ctf/kubernetes-privilege-escalation-from-pod-access-to-cluster-c).

### Path C: Docker Security & Forensics
1. **Hardening & Management:** Master container isolation using [Docker Compose Security](https://learn.secbyte.org/ctf/docker-compose-security) and [Docker Secrets](https://learn.secbyte.org/ctf/docker-secrets-securely-managing-sensitive-data-in-container).
2. **Investigation & Response:** Execute DFIR workflows in [Docker Forensics](https://learn.secbyte.org/ctf/docker-forensics-investigating-containerized-intrusions) and [Docker Incident Response](https://learn.secbyte.org/ctf/docker-incident-response-investigate-contain-eradicate).

---

## How to Use the Labs

1. Select a practice scenario from the **Lab Collection Index**.
2. Click the direct link to launch the exercise environment on Learn SecByte.
3. Review scenario topology, challenge goals, and target constraints.
4. Execute terminal commands, analyze container artifacts, or remediate misconfigurations to locate flags.

---

## Target Audience

* **DevSecOps Engineers & Cloud Architects:** Master container isolation, security standards, and automated deployment hardening.
* **Penetration Testers & Red Teams:** Practice container escape techniques, RBAC abuse, and cluster takeover vectors.
* **DFIR & SOC Responders:** Learn specialized digital forensics and incident response techniques for containerized infrastructure.
* **Cybersecurity Students:** Gain practical cloud-native skills through interactive training environments.

---

## Disclaimer

All lab links in this repository direct to authorized exercises hosted on Learn SecByte. These materials are provided strictly for educational purposes, defensive skill building, and security research. Unauthorized testing against external systems or clusters is strictly prohibited.
