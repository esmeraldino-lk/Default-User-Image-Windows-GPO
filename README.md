# Default-User-Image-Windows-GPO


1. Make a 448x448,192x192,48x,40x,32x BMP, PNG and JPG image.
2. Make a folder, shared or not to other pcs access it. Ex: \\server\files\images\user\
3. Place previous images to this folder.
4. Open Group Policy Management.
5. Create a new Policy.
6. Go to tab **COMPUTER CONFIGURATION > POLICIES > ADMINISTRATIVE TEMPLATES > CONTROL PANEL > USER ACCOUNTS** ![image](https://github.com/esmeraldino-lk/Default-User-Image-Windows-GPO/assets/133903212/75bc8d8a-c9a7-4a90-87df-73c921759318)

7. Enable **APPLY THE DEFAULT ACCOUNT PICTURE TO ALL USERS**
8. Go to tab **COMPUTER CONFIGURATION > PREFERENCES > WINDOWS SETTINGS > FILES**
9. Create the follow rule to this files:
    
        ACTION: **REPLACE**
        SOURCE FILE: ***\\server\files\images\user\***
        DESTINATION FILE: ***%PROGRAMDATA%\Microsoft\User Account Pictures\user.jpg***

10. Do that to the follow files:
    1. user.jpg
    2. user.png
    3. user.bmp
    4. user-192.png
    5. user-48.png
    6. user-40.png
    7. user-32.png
    8. guest.bmp
    9. guest.jpg
![image](https://github.com/esmeraldino-lk/Default-User-Image-Windows-GPO/assets/133903212/9e705537-f757-4ee2-9603-35e53aee07e1)
