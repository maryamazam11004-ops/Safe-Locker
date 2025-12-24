SafeLocker 

SafeLocker is a mobile application designed to securely store photos, videos, audio files and documents by encrypting them locally on the user’s device.  
The app also provides backup & sync support using Supabase, so that users can restore their encrypted data if the device is lost or replaced.

 Key Features

✔ Local AES Encryption All files are encrypted inside the device before storage  
✔ Master Password Protection App unlocks only with user's master password  
✔ Optional Recovery Key Used to recover access if password is forgotten  
✔ Decoy Vault (Fake Password) Opens a fake vault to protect user under pressure  
✔ Offline First Works fully offline except for cloud backup & sharing  
✔ Secure Cloud Backup (Supabase) Only encrypted files are stored on cloud  
✔ File Types Supported
• Images • Videos • Audio • Documents  


 Security Model (Simple Explanation)

  A Master Password → derives an Encryption Key
  Files are encrypted locally using AES-256
  Only encrypted files are uploaded to Supabase
  Supabase NEVER sees the real password or decrypted files
  Recovery Key is stored safely by the user to reset password



 Why SafeLocker?

Most “calculator vault” apps only hide files.  
SafeLocker encrypts them  meaning even if:

✔ phone is stolen  
✔ SD card is removed  
✔ cloud server is hacked  

your files stay unreadable.


Tech Stack

Flutter – Mobile App
Supabase– Authentication + Encrypted File Backup
AES-256– File Encryption


 Authentication Flow

1️⃣ User signs up / logs in with email (Supabase)  
2️⃣ User sets Master Password 
3️⃣ Files are encrypted using key derived from password  
4️⃣ Encrypted files are stored locally + optional cloud backup  
5️⃣ To unlock vault → master password required



 Password Recovery Options

Recovery Key (Recommended & Secure)  
(Optional) Email-based recovery with security warning


Storage Options

User can choose:
Internal Storage (default)
SD Card (encrypted files only)



 Status

 Student Academic Project  
 Under development  
 For learning & research purposes  



