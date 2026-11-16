# Reviewing-Unallocated-Space-Extracting-Data-with-Tools-Digital-Investigation-Processes
## AIM:
To review unallocated space in a disk image, extract data using forensic tools, and understand the digital investigation process.
## REQUIREMENTS
- Autopsy or FTK Imager
- Sleuth Kit (TSK)
- Hex Editor (e.g., HxD)
- Operating System: Windows 10/11 or Linux (Kali preferred)
## ARCHITECTURE DIAGRAM
```mermaid
flowchart TD
    A[Disk Image / Physical Drive] --> B[Load into Autopsy or Sleuth Kit]
    B --> C[Identify Unallocated Space]
    C --> D[Scan for Data Signatures]
    D --> E[Carve and Recover Files]
    E --> F[Analyze Recovered Data]
    F --> G[Document Findings in Report]
```
## DESIGN STEPS:
### Step 1 (Acquire Evidence Image):
- Obtain the disk image in ```.dd``` or ```.E01``` format from a trusted forensic acquisition process.
- Verify hash values (MD5/SHA256) to maintain integrity.

### Step 2(Load Image into Forensic Tool):
- Open Autopsy or FTK Imager.
- Create a new case and add the evidence image.

### Step 3(Locate Unallocated Space):
- Navigate to the partition structure view.
- Identify sectors not assigned to any partition (unallocated).
### Step 4(Analyze & Carve Data):
- Use built-in data carving tools to search for file signatures (JPEG, DOCX, PDF, etc.).
- Preview carved files for relevance.
  
## PROGRAM:
| Step | Action                     | Tool Used                   | Output                       |
| ---- | -------------------------- | --------------------------- | ---------------------------- |
| 1    | Load disk image            | Autopsy / FTK Imager        | Partition & unallocated view |
| 2    | Identify unallocated space | Autopsy File System View    | Sector ranges                |
| 3    | Data carving               | Autopsy Data Carving Module | Recovered files              |
| 4    | Export evidence            | Autopsy Export Option       | File copies for analysis     |


## OUTPUT:
Unallocated Space Analysis and Extracted Data Report
<img width="838" height="430" alt="image" src="https://github.com/user-attachments/assets/a8b25575-e896-486d-8dd7-d5b382eef451" />
<img width="839" height="431" alt="image" src="https://github.com/user-attachments/assets/c3c31c16-772e-4ea6-9941-a84f0adcac53" />
<img width="837" height="430" alt="image" src="https://github.com/user-attachments/assets/c1a209aa-4bc2-45c0-b738-134900a8de32" />
<img width="837" height="433" alt="image" src="https://github.com/user-attachments/assets/b9d93c7a-88c7-4447-855f-676428c8317f" />
<img width="835" height="438" alt="image" src="https://github.com/user-attachments/assets/b5ed64fd-e21f-4585-b8f9-7329fa6e1bc2" />
<img width="836" height="406" alt="image" src="https://github.com/user-attachments/assets/3c85a28d-6816-4e5c-99ef-5fb9ec5fd58c" />
<img width="842" height="364" alt="image" src="https://github.com/user-attachments/assets/4e378876-fcbb-49cf-83b2-b3c4196a3ebc" />

## RESULT:
The unallocated space was successfully analyzed, data was extracted, and the digital investigation process was followed effectively.

