### Instance Sanity Check Automation

**Problem:**  
Customers required validation of application availability from an end-user perspective. A legacy jMeter-based solution was in place, but it had multiple challenges:  

1. Engineers had to manually keep their jMeter test plans updated.  
2. Each engineer needed Java, jMeter, and dependencies installed locally.  
3. The process was slow (2–4 minutes per instance) and manual verification of returned content made major incident checks (30–50 instances) extremely time-consuming.  

**Solution:**  
I developed a centralized UI-driven tool to automate and streamline instance checks:  

- **Frontend (HTML + JS):** Rendered a list of instances, allowing simultaneous execution of sanity checks.  
- **Backend (PHP):** Launched jMeter processes asynchronously and automatically validated returned content against key phrases.  
- **Reporting:** Produced a dynamic report highlighting which parts of the application failed expected content checks.  

**Impact:**  
- Reduced validation of the entire customer fleet (30–50 instances) to **5–10 minutes total**.  
- Eliminated dependency on each engineer managing their own jMeter setup.  
- Provided standardized, consistent validation across the department.  
- The tool was widely adopted, remained in use long after my departure, and eventually inspired a more modern implementation using Puppeteer — keeping the same core idea I introduced.  

**Tech Stack:**  
- HTML, JavaScript (frontend)  
- PHP (backend execution & orchestration)  
- jMeter (test automation)  
