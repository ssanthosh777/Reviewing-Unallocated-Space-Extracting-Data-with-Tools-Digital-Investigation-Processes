# Reviewing-Unallocated-Space-Extracting-Data-with-Tools-Digital-Investigation-Processes
```
NAME: SANTHOSH S
REG.NO: 212224100052
```
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
<img width="1920" height="1200" alt="Screenshot (51)" src="https://github.com/user-attachments/assets/02c93b4a-dcbc-46da-bab4-fe8077ad9633" />
<img width="1920" height="1200" alt="Screenshot (52)" src="https://github.com/user-attachments/assets/f9e27e14-30c3-4260-a341-ea5d6cda26e9" />
<img width="1920" height="1200" alt="Screenshot (50)" src="https://github.com/user-attachments/assets/9e631cd6-bef8-459c-af50-c1cebc399d04" />


<img width="1920" height="1080" alt="Screenshot (53)" src="https://github.com/user-attachments/assets/02d8bdf0-039e-4d3e-909c-3360159d2d96" />
<img width="1920" height="1080" alt="Screenshot (54)" src="https://github.com/user-attachments/assets/0676235b-5cce-43b5-b7f7-f613b499fd87" />
<img width="1920" height="1200" alt="Screenshot (55)" src="https://github.com/user-attachments/assets/f84148df-27ff-49ec-bb85-1c6c9aa94578" />
<img width="1920" height="1200" alt="Screenshot (56)" src="https://github.com/user-attachments/assets/b5ff6e04-7099-4f44-a462-7c207f2c4d21" />
<img width="1920" height="1200" alt="Screenshot (49)" src="https://github.com/user-attachments/assets/95541826-bceb-486a-adc3-8ee4293dbcf8" />

## RESULT:
The unallocated space was successfully analyzed, data was extracted, and the digital investigation process was followed effectively.

