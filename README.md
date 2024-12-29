# ELK Stack Deployment and Monitoring

## Project Overview
This project involves the deployment of the ELK Stack (Elasticsearch, Logstash, Kibana) on Vultr cloud infrastructure for real-time monitoring and security analysis of Ubuntu and Windows servers. By using Elastic Fleet Server and agents, we detect and analyze suspicious activities, such as RDP authentication failures and SSH brute force attacks.

---

## Features
- **Real-Time Monitoring:**
  - Track logs and system events on Ubuntu and Windows servers.
- **Custom Alerts:**
  - Set up alerts for specific activities, such as failed login attempts.
- **Data Visualization:**
  - Use Kibana to create dashboards and maps for log analysis.
- **Cloud Infrastructure:**
  - Host servers on Vultr for scalability and flexibility.

---

## Project Architecture
- **Servers:**
  - Ubuntu server for hosting Elasticsearch.
  - Windows server as the monitored system.
- **Tools:**
  - Elasticsearch for log storage and search.
  - Kibana for visualization and alerting.
  - Elastic Agent and Fleet Server for monitoring.

![Logical Diagram](path/to/logical-diagram.png) *(Replace with actual path if applicable)*

---

## Setup Instructions

### Prerequisites
- Vultr account.
- Ubuntu and Windows server instances.
- Basic knowledge of command-line tools.

### Steps
1. **Set Up Vultr Environment:**
   - Create virtual machines with assigned IPs.
   - Configure Ubuntu and Windows instances.

2. **Install Elasticsearch:**
   - Update the Ubuntu server.
   - Install Elasticsearch using package manager.
   - Configure `elasticsearch.yml` file.

3. **Install Kibana:**
   - Install Kibana on the Ubuntu server.
   - Generate and use an enrollment token for authentication.

4. **Deploy Elastic Agent and Fleet Server:**
   - Install and configure the Elastic Fleet Server.
   - Connect the Windows server as an agent.

5. **Visualize and Monitor:**
   - Use Kibana dashboards to analyze logs and create custom alerts.

---

## Monitoring Activities
- **RDP Authentication Logs:**
  - Detect and analyze failed login attempts using event ID 4625.
- **SSH Brute Force Attacks:**
  - Monitor failed login attempts with source IPs and locations.

---

## Future Enhancements
- Integrate machine learning for anomaly detection.
- Expand monitoring to additional server types.
- Automate response to detected threats.

---

## Contributing
Feel free to fork this repository and contribute to the project. Submit a pull request with your suggestions or improvements.

---

## License
This project is licensed under the MIT License. See the LICENSE file for details.
