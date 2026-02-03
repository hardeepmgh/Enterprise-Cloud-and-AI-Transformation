## Day 12: The Cloud Landing Zone & Hybrid Data Pipeline

### ✅ Accomplishments:
- **Infrastructure as Code:** Deployed a full AWS VPC with Public/Private Subnets and an RDS PostgreSQL instance using **Terraform**.
- **Database Architecture:** Configured `pgvector` for future AI-ready vector searches.
- **Hybrid Connectivity:** Established a secure connection between a local MacBook and a cloud-hosted RDS instance using Security Group ingress rules.
- **Data Ingestion:** Successfully bypassed local environment Segmentation Faults (x86_64 architecture conflicts) by implementing a lightweight Python ingestion pipeline.
- **Verification:** Successfully retrieved data from AWS via a Python search script.

### 🛠️ Tech Stack Used:
- **Terraform** (IaC)
- **AWS** (VPC, RDS, Subnets, IGW)
- **PostgreSQL** (with pgvector)
- **Python** (psycopg2)

### 📈 Current Status:
Infrastructure verified and decommissioned via `terraform destroy`. 
**Data Persistence Success:** 100%
