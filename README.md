# Detecting-steganography-with-tools-like-StegExpose-analyzing-file-signatures
## AIM:
To detect hidden data using steganography detection tools like StegExpose and analyze file signatures for authenticity and manipulation.

## DESIGN STEPS:
### Step 1:
Install StegExpose or use the JAR version to detect steganography in image files.

### Step 2:
Run StegExpose on a directory of suspected image files using the command:

### Step 3:
Analyze file signatures using tools like file, binwalk, or xxd to check for inconsistencies or embedded content.

## PROCEDURE:
StegExpose and File Signature Analysis Commands

## Step 1: Download Image and Create Secret Message File
• Download a .jpeg image from a trusted website or use own image.

![436934288-e8d88fc9-6cd0-4d71-87ed-300ceee7ab29](https://github.com/user-attachments/assets/3ac002af-5f35-4e61-ac99-8fed3d01aebe)


• Create a text file named secret with a confidential message:

![436934459-d97fe8bf-c605-4f69-9ef4-6d991c48c73e](https://github.com/user-attachments/assets/b1f4374e-d2cf-4ebd-8914-e68ebce9dded)


## Step 2: Install and Verify Steghide Tool

• To install Steghide on Kali linux,run:

• Confirm the installation by checking its version:

![436934836-a10a04a2-6266-4a5c-98e5-e4e331318e81](https://github.com/user-attachments/assets/82cfa596-bcb0-4547-8cde-ae00f7cf1424)


## Step 3: Embed the Secret Message into the Image
• Use the following command to embed secret into praveen.jpeg:

![436935023-0b461cbe-10e5-4f1f-a272-240f39ed531d](https://github.com/user-attachments/assets/4bf46955-8dc7-47b4-817d-9b8ee2a4d9b6)


## Step 4: Delete the Original Secret File
• After embedding, delete the plaintext file:

![436935378-a3bb37c5-8e86-4b53-a869-2a26ca227244](https://github.com/user-attachments/assets/6f96cbfc-95db-494d-894e-9d10484c1296)


## OUTPUT:
List of Images with Steganography Detection Scores and File Signature Details

## Step 1: Extract the Embedded Secret from the Image

![436935692-4c39d9c7-92a9-4081-b40d-ea5540e94c49](https://github.com/user-attachments/assets/e954517c-af98-41b2-a911-4cf2f47ce7a5)

• To retrieve the hidden file: • Enter the same passphrase used during embedding.

![436936087-b7da3f33-4d8c-4fa0-9349-dbc28d944d53](https://github.com/user-attachments/assets/0a209b46-302f-407a-bd3d-829acb7e532d)


## Step 2: Verify the Extracted Message
• Display the extracted file content to verify:

• Ensure the message matches the original secret content.

• Another command to see the same secret message is

## Step 3: Retrieve Information About the Embedded Data
• To gather details about embedded content in the image:

![436936595-9a499ab3-50fd-4a9d-a08f-5a01eca456b8](https://github.com/user-attachments/assets/a2b569ce-180e-4c55-97e4-6a335c77c769)

• This will display file type, size, and whether data is embedded.

## RESULT:
Hidden data was successfully detected and file signatures were analyzed for irregularities.
