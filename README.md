<img width="837" height="446" alt="image" src="https://github.com/user-attachments/assets/871d767c-1e91-44d8-a183-b911ccfd0c22" /># Reviewing-Unallocated-Space-Extracting-Data-with-Tools-Digital-Investigation-Processes
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
<img width="1598" height="839" alt="image" src="https://github.com/user-attachments/assets/c4498ed3-07b1-469b-aff0-5db69fc65efb" />
<img width="1600" height="834" alt="image" src="https://github.com/user-attachments/assets/4b952af4-7019-43cd-9314-52becbfcad86" />
<img width="1600" height="687" alt="image" src="https://github.com/user-attachments/assets/2f730137-c98f-403f-87b2-6c3ff3f9b842" />
<img width="1600" height="734" alt="image" src="https://github.com/user-attachments/assets/51476119-5014-4b68-b95b-5df518a8b394" />
<img width="1600" height="849" alt="image" src="https://github.com/user-attachments/assets/d536c865-6bf0-40e3-a763-3f3e72e847bd" />
<img width="594" height="270" alt="image" src="https://github.com/user-attachments/assets/15cfbb94-ee7a-4192-b8e0-c5dbaff0c33f" />
<img width="838" height="362" alt="image" src="https://github.com/user-attachments/assets/67f86389-f58c-4707-830c-ea1e71764590" />







## RESULT:
The unallocated space was successfully analyzed, data was extracted, and the digital investigation process was followed effectively.

