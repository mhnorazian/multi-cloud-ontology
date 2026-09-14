# Semantic Multi-Cloud Ontology

This repository provides a modular ontology architecture designed to enable **semantic interoperability** across **multi-cloud platforms**, specifically between **AWS** and **OpenStack**.

The ontologies support both:
- **Horizontal Interoperability**: across cloud providers (AWS and OpenStack)
- **Vertical Interoperability**: across service layers (IaaS → PaaS → SaaS)

---

## 📂 Repository Structure

multi-cloud-ontology/
├── ontologies/
│   ├── cloud-interoperability-core.ttl   # Provider-agnostic core ontology
│   ├── aws-cloud.ttl                     # AWS-specific service taxonomy
│   ├── os-cloud.ttl                      # OpenStack-specific service taxonomy
│   ├── cloud-mapping.ttl                 # Decoupled semantic rules & symmetric equivalence
│   └── cloud-instances.ttl               # Populated benchmark dataset (62 individuals)
│
├── queries/                              # SPARQL competency query suite
│   ├── q1_compute_discovery.rq           # Multi-attribute VM filtering (vCPU ≥ 1, Cost < $0.05/hr)
│   ├── q2_database_discovery.rq          # Managed relational database filtering (Cost < $0.03/hr)
│   ├── q3_storage_discovery.rq           # Object storage service retrieval (S3 & Swift)
│   ├── q4_qos_cost_filtering.rq          # Multi-attribute SLA filtering (Availability ≥ 99.9%)
│   ├── q5_functional_equivalence.rq      # Direct symmetric equivalence mapping validation
│   ├── q6_regional_location.rq           # Region and location-aware multi-cloud filtering
│   ├── q7_price_performance_ratio.rq     # Price-performance ratio ranking (vCPUs per dollar)
│   └── q8_memory_capacity_filter.rq      # Hardware RAM capacity filtering (RAM ≥ 4 GB)
│
├── docs/
│   ├── Ontology-Diagram.png              # Visualization of class hierarchy and properties
│   ├── Class_Hierarchy_Asserted.png     # Asserted class hierarchy diagram
│   ├── Class_Hierarchy_Inferred.png     # Inferred class hierarchy diagram
│   ├── OntologyMetrics.png              # Protégé ontology metrics screenshot
│   └── HermiTReasoner_Log.png           # Protégé HermiT reasoning execution log
│
├── LICENSE                               # CC license
└── README.md                             # This file
