### Oracle Field Service Forms Viewer

**Problem:**  
Export/import operations in Oracle Field Service (OFS) require the target instance to contain all properties from the source. Troubleshooting mismatches is time-consuming, especially when analyzing exported data manually.  

**Solution:**  
I developed a JavaScript-based viewer that recursively processes OFS export data and replicates OFS-like visuals, including visibility rules for nested elements.  

- **Local & Secure:** All data is processed entirely in the browser session — no uploads, ensuring sensitive configuration remains private.  
- **Lightweight Deployment:** To minimize footprint, the JS code was transformed into standalone HTML and embedded directly into a Confluence page, requiring no external hosting or backend.  

**Impact:**  
The tool significantly accelerated troubleshooting by enabling **instant, secure visualization of exported OFS data**, reducing dependency on time-consuming manual checks.  

**Tech Stack:**  
- JavaScript (DOM manipulation, recursive parsing)  
- HTML (self-contained deployment)  
- Confluence integration  
