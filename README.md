# EXP8:DETECTING STEGANOGRAPHY WITH TOOLS  LIKE STEGEXPOSE,ANALYSING FILE SIGNATURES

## AIM:
To hide and extract secret information (e.g., text files) inside a cover file (e.g., JPEG image) using the steganography tool `steghide` in Kali Linux.

EQUIPMENTS REQUIRED:
●	Hardware: PCs

```
Register Number: 212222040095
Name: Mahisha S
```

## DESIGN STEPS:
### Step 1:
Install StegExpose or use the JAR version to detect steganography in image files.

### Step 2:
Run StegExpose on a directory of suspected image files using the command:

### Step 3:
Analyze file signatures using tools like file, binwalk, or xxd to check for inconsistencies or embedded content.

## PROCEDURE:
### Step 1: Download Image and Create Secret Message File
  •	Download a .jpeg image (e.g., praveen.jpeg) from a trusted website or use own image.
  
  ![Screenshot 2025-04-22 180246](https://github.com/user-attachments/assets/2647b024-ce12-4905-a888-e7c382e80036)

  
  •	Create a text file named secret with a confidential message:
  
  ![Screenshot 2025-04-22 180507](https://github.com/user-attachments/assets/4cb60ba6-a5f9-4da0-a4c0-7e0729470cc7)

  ![Screenshot 2025-04-22 180542](https://github.com/user-attachments/assets/dc069feb-464d-46e3-a61b-ecb5f17be7fc)



### Step 2: Install and Verify Steghide Tool
  •	To install Steghide on Kali linux,run:
  
  ![Screenshot 2025-04-22 180734](https://github.com/user-attachments/assets/20ed1909-5b42-44f0-ab82-133e461c4acd)

  
  •	Confirm the installation by checking its version:
  
  ![Screenshot 2025-04-22 180755](https://github.com/user-attachments/assets/597a1b6a-6b08-4eae-8abc-cefcedfc7806)


 
### Step 3: Embed the Secret Message into the Image
  •	Use the following command to embed secret into praveen.jpeg:
  
  ![Screenshot 2025-04-22 181002](https://github.com/user-attachments/assets/79138996-8352-4c57-80c6-8d35f6290980)




### Step 4: Delete the Original Secret File
  •	After embedding, delete the plaintext file:
  
  ![Screenshot 2025-04-22 181054](https://github.com/user-attachments/assets/bb4fc96b-d642-4fb0-9cc0-41addce20c6d)


## OUTPUT:
### Step 1: Extract the Embedded Secret from the Image
  •	To retrieve the hidden file:
  
  ![Screenshot 2025-04-22 181208](https://github.com/user-attachments/assets/9932925f-65ee-4921-8d15-a6222c1d623f)


  •	Enter the same passphrase used during embedding.
  
  ![Screenshot 2025-04-22 181315](https://github.com/user-attachments/assets/4cd8f69b-018b-4635-8b42-adc18c86ac19)



### Step 2: Verify the Extracted Message

  •	Display the extracted file content to verify:
  
  ![Screenshot 2025-04-22 181343](https://github.com/user-attachments/assets/d233fcda-625d-41e1-a6c0-966a88c57292)

  
  •	Ensure the message matches the original secret content.
  
  •	Another command to see the same secret message is
  
  ![Screenshot 2025-04-22 181406](https://github.com/user-attachments/assets/004de896-9c72-4350-ac40-23f3ab9bc222)


 
### Step 3: Retrieve Information About the Embedded Data
  •	To gather details about embedded content in the image:
  
  ![Screenshot 2025-04-22 181555](https://github.com/user-attachments/assets/323daf00-0b81-4032-9c08-a7b6c6164f5f)

  
   
  •	This will display file type, size, and whether data is embedded.

 
## RESULT:
Embedded "secret" into praveen.jpeg successfully using Steghide with passphrase 12345.Extracted and verified hidden message
