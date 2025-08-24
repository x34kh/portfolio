### Custom Deployment Automation with Ansible & Telegram Bot

To meet the business owner’s requirement for granular control over production releases, I designed and implemented a custom deployment solution instead of a traditional CI/CD pipeline with automated deployment.  

- **Infrastructure Automation:**  
  Developed Ansible scripts to pull Java source code from GitHub, build it on a dedicated Maven server, and deploy compiled artifacts to production instances.  

- **Custom Control Interface:**  
  Built a Telegram bot (Python) serving as the user interface, enabling controlled execution of deployment tasks with role-based access control (RBAC).  

- **Robust Architecture:**  
  Implemented the bot as a multithreaded application with message queues and safeguards against conflicting executions. Integrated it with a Flask-based API to trigger Ansible playbooks securely.  

![telegram_bot_example](https://github.com/user-attachments/assets/a180b0d8-34f8-45ae-9c77-d7bd5a07b3fa)  

**Impact:**  
This solution gave the business a **reliable, non-technical-friendly deployment workflow**, reducing dependency on engineers while maintaining full control and traceability of production releases. It combined automation efficiency with the manual oversight required by stakeholders.  

**Tech Stack:**  
- **Languages & Frameworks:** Python, Flask, Java, Maven  
- **Automation & Orchestration:** Ansible  
- **Messaging & UI:** Telegram Bot API  
- **Infrastructure:** Dedicated build server (Linux, Docker), production instances (Docker, Tomcat)
