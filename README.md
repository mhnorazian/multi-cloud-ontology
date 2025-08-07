# Semantic Multi-Cloud Ontology

This repository provides a 2-layer ontology architecture designed to enable **semantic interoperability** across **multi-cloud platforms**, specifically between **AWS** and **OpenStack**.

The ontologies support both:
- **Horizontal Interoperability**: across cloud providers
- **Vertical Interoperability**: across service layers (IaaS → PaaS → SaaS)

---

## 📂 Repository Structure

multi-cloud-ontology/
├── ontologies/
│ ├── core-cloud.ttl # Main core ontology
│ ├── aws-cloud-mapped.ttl # AWS-specific services mapped to core
│ └── os-cloud-mapped.ttl # OpenStack services mapped to core
│
├── examples/
│ └── sample-service-query.rq # Example SPARQL query
│
├── docs/
│ └── ontology-diagram.png # Visualization of ontology
│
├── LICENSE # CC license
└── README.md # This file
