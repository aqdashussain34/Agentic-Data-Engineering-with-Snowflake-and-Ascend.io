**Agentic Data Engineering with Snowflake and Ascend.io**
📌 **Project Overview**
This project demonstrates the transition from manual data orchestration to Agentic Data Engineering. Using the Ascend.io platform, I architected an automated data lifecycle that handles ingestion, transformation, and predictive analytics natively on a Snowflake data cloud.

🛠️ **Phase 1: Infrastructure & Security**
The foundation of this project was establishing a secure connection between Ascend and Snowflake.

**RSA Key-Pair Authentication:** Instead of basic passwords, I configured high-security RSA authentication.

**Secure Credential Management:** Encrypted private keys were managed via the Ascend Environment Vault, ensuring that sensitive credentials never appeared in plain text within the pipeline code.

**Data Plane Integration:** Successfully validated the Snowflake Data Plane, allowing Ascend to leverage Snowflake's compute power for all SQL transformations.

🤖 **Phase 2: Agentic Pipeline Development**
Rather than writing thousands of lines of manual orchestration code, I utilized Otto, an AI-driven data engineering assistant.

**Data Ingestion**
Connected to real-time and synthetic datasets, including goats.csv and local weather/carbon APIs.

Configured automated File Readers to monitor source locations for new data.

**Transformations**
**SQL Transforms:** Built modular SQL logic to aggregate metrics like carbon by day of week and weather-categorized forecast data.

**Python Transforms:** Integrated custom Python logic for advanced data enrichment, such as calculating performance tiers and revenue metrics.

📈 **Phase 3: Orchestration & Analytics**
The final stage involved turning raw data into actionable business intelligence.

**Predictive Analytics:** Developed a carbon_predictions flow that utilizes historical data to forecast future carbon trends.

**Automated Scheduling:** Set up the pipeline to run on automated schedules, ensuring the final dashboard is always updated with the freshest data.

**Intelligent Error Handling:** Configured the agentic system to respond to upstream failures, providing a "self-healing" data environment.

💻 **Technical Stack**
Platform: Ascend.io (Agentic Data Engineering)

Data Warehouse: Snowflake

Languages: SQL, Python, YAML

Security: RSA Key-Pair, Instance Vault

CI/CD: GitHub Integration for Pipeline-as-Code

✅ **Final Results**
By the end of the project, I successfully deployed a fully automated data ecosystem. The final result is a real-time dashboard that visualizes carbon and weather insights, proving that AI agents can significantly reduce the complexity of modern data engineering.
