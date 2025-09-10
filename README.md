# FILE-RECOVERY-USING-AUTOPSY-SOFTWARE

## AIM
To use **Autopsy Digital Forensics Tool** to retrieve deleted files from a disk image.

---

## REQUIREMENTS
- **Operating System**: Windows 10/11, macOS, or Linux
- **Tool**: [Autopsy Digital Forensics](https://www.autopsy.com/)  
- **Test Data**: Disk image file (`disk.dd`, `disk.img`, `.E01`)

---

## ARCHITECTURE DIAGRAM

<img width="577" height="785" alt="Screenshot 2025-08-22 151258" src="https://github.com/user-attachments/assets/0e9e4744-5534-4828-8715-d6210ba065c3" />

## DESIGN STEPS:
### Step 1:
Open Autopsy and create a new case with appropriate case details.

### Step 2:
Add a disk image as a data source and let Autopsy analyze the content.

### Step 3:
Navigate to the "Deleted Files" section in Autopsy and examine or recover the deleted files.

## PROGRAM:
### **1. Copy Files to the Virtual Disk**  
- Open **File Explorer** → Go to the new drive (`C: or D:`), where the folder created in the New Virtual Disk
- Create a new folder (`Autospy`) and copy **images or files** into it.  

### **2. Delete the Files**  
- Select any one or two images → Press **Delete**.  
- Empty the **Recycle Bin** to permanently delete them.  

### **3. Recover Deleted Files Using Autopsy**  
### **Open Autopsy & Create a New Case** 

- Launch **Autopsy** and **Run as a administrator**  
- Click **Create New Case**.  

<img width="612" height="421" alt="a1" src="https://github.com/user-attachments/assets/b708135b-a982-48cd-a201-7bf8d571e78e" />

- Enter a **Case Name** (e.g., `Autopsy1`).  
- Choose a **Case Folder** location.  
- Click **Next** → Click **Finish**.  

<img width="976" height="573" alt="a2" src="https://github.com/user-attachments/assets/d1aafe35-8191-489d-9633-c7a1d4027958" />


### **Add the Virtual Disk as an Evidence Source**  
- Click **Add Data Source**  → **Select Host**

<img width="1070" height="673" alt="a3" src="https://github.com/user-attachments/assets/64e38d5d-35b1-42ee-af04-a07705af103f" />


- Select **Local Disk** → **next** 

<img width="1070" height="667" alt="a4" src="https://github.com/user-attachments/assets/afaabfeb-e422-4f9b-abce-d8a1178f8525" />


- Select Disk → **Choose the VHD drive (`Drive1`)**

<img width="1057" height="665" alt="a5" src="https://github.com/user-attachments/assets/aa0aea29-82bf-49e0-8aa2-e97fdb3c42d2" />


- Click **Next** → Keep default settings → Click **Finish**.  
- Wait for Autopsy to process the disk.  

### **Recover Deleted Files**  
- Go to **File Views** (left panel).  

<img width="1256" height="679" alt="image" src="https://github.com/user-attachments/assets/9ee0b009-5c81-4b20-a2c6-ffa38355d130" />


- Click **Deleted Files** → Find your deleted images.  
- Right-click an image → Click **Extract File**.  

- Select a folder to see the recovered files (e.g., `C:\forensic`).  
- Image is recovered successfully.


## Output :


### Folder before deleting the files

![image1](https://github.com/user-attachments/assets/ce17a5ca-6da0-4164-8fa9-f59b738abbcf)

### Folder after deleting the files
![image 3](https://github.com/user-attachments/assets/f96ca485-929f-4084-9289-fbe1d2b966b6)


### Folder after extracting the deleted images using autopsy

<img width="884" height="479" alt="image" src="https://github.com/user-attachments/assets/d66954e2-7c56-47fb-897e-670daa810a3f" />


## RESULT:

Deleted files were successfully retrieved and analyzed using Autopsy.

