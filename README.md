# MOBYDICK
HELP TO GET ACCESS TO MOBYDICK.OVH

## COMMANDS TO REMEMBER 

(this is for future you, if i dont code an interface)

| COMMAND LINE | PURPOSE | EXEMPLE |
|  :-: | :-: | :-: |
| `git clone` | Clone a project locally | git clone git@mobydick.ovh:mobydick/cowbot.git |
| `git status` | Get the difference between the local version and the server version | - |
| `git pull` | Download the difference between the server and the local version | - |
| `git add` | Make Git Track the file you want to upload | git add test.txt // git add . |
| `git commit` | Make all files tracked part of the next Push // (-m is **OBLIGATORY** and is the title of your Push - Should be easy to understand) | git commit -m "TEST" |
| `git push` | Upload to the server all add and comitted files | - |


## 1 : CREATE AN ACCOUNT INTO MOBYDICK.OVH

GO TO :: [MOBYDICK](https://mobydick.ovh/users/sign_up)

![image](https://github.com/FrenchFive/mobydick/assets/105274118/d651e43a-c2be-42cf-a26c-834478f33d33)

> [!IMPORTANT]
> **ACCOUNT NEEDS TO BE ACCEPTED BY AN ADMIN** (aka. Five for now) >> **SEND THEM A MESSAGE**
> <br> [This is for Security maesures for now ...] 

![image](https://github.com/FrenchFive/mobydick/assets/105274118/9a3cc364-c48b-4219-998a-560dde787c7a)

---

## 2 : INSTALL GIT

GO TO :: [GIT](https://git-scm.com/download/win)
<br> And download Git for Windows (if you are on Windows)

![image](https://github.com/FrenchFive/mobydick/assets/105274118/c1399ef4-a393-43ed-b208-a3ed234893a7)

> [!NOTE]
> **EVERYTHING AS DEFAULT WORKS PERFECTLY**
> <br> No need to open it at the end, nor to open the webpage

---

## 3 : CREATE AN SSH KEY

Just so you know : Passwords are cool, but can be cracked, the goal here is to generate a unique key that your computer and the server will have, instead of typing your password, the server will ask for your key and compare it to the server. If they match, then you'll be able to edit and change things as you want from command lines without having to go through the website.

OPEN :: **WINDOWS POWERSHELL**
<br> TYPE :
```batch
ssh-keygen
```
![image](https://github.com/FrenchFive/mobydick/assets/105274118/7f66183c-b873-48fd-874c-b7f5ca73eca7)

> [!TIP]
> Giving the ASKED INFORMATION IS **FACULTATIVE**. 
> <br> You can skip it by pressing the "Enter" Key.

We want to get the key and copy it to the website.
<br> STILL IN THE **POWERSHELL**
<br> TYPE : 
```batch
cat ~/.ssh/id_rsa.pub
```
![Sans titre-1](https://github.com/FrenchFive/mobydick/assets/105274118/e2a576f4-4adc-4833-bc1e-7ca8bfe976f0)

COPY THE OUTPUT.
<br> Including "ssh-rsa ..."

ONCE ACCEPTED ON THE WEBSITE.
<br> LOGIN :: [LOGIN PAGE](https://mobydick.ovh/users/sign_in)

![image](https://github.com/FrenchFive/mobydick/assets/105274118/568bc404-6a1e-4aa4-beb6-537f4f056be2)

GO INTO YOUR PREFERENCES.

![image](https://github.com/FrenchFive/mobydick/assets/105274118/a9fd8262-cb40-434c-ac8d-22008add9bfa)

![image](https://github.com/FrenchFive/mobydick/assets/105274118/a73a2ad9-6732-4769-9d79-244eab2bcbf4)

AND ADD A NEW KEY

![image](https://github.com/FrenchFive/mobydick/assets/105274118/3c097db1-ca91-4d9e-950e-1ec640c3d6e5)

PASTE YOUR COPIED KEY INTO THE FIELD

YOU SHOULD GET THIS :

![Sans titre-1](https://github.com/FrenchFive/mobydick/assets/105274118/5b89bd48-da36-4ec7-bf81-1147c05e3923)

---

## 4 : CLONE THE PROJECT

If the admin worked properly, he added you to your group. 
<br> Or you can create your own.
<br> Create projects ... etc ... 

![image](https://github.com/FrenchFive/mobydick/assets/105274118/298ef135-6e73-4f4e-934a-d68df79cee91)

ONCE YOU PICKED A PROJECT YOU WANT TO CLONE 
<br> CLICK ON CODE > COPY THE SSH LINK

![image](https://github.com/FrenchFive/mobydick/assets/105274118/32c0e50a-ab6f-4151-a7cf-96ee267b7a5c)

SELECT THE FOLDER YOU WANT THE PROJECT TO BE AT
<br> Option 1 : SIMPLE : Right Click in the File Explorer and Select "Open in the Terminal"

![image](https://github.com/FrenchFive/mobydick/assets/105274118/bc4c5db5-9944-4a8c-8dd9-7807c7198ce9)

Option 2 : CODE : Open the **POWERSHELL**
<br> Copy the path to your directory [Your path needs to exists already]
<br> TYPE : 
```batch
cd D:\YOUR\PATH
```
![image](https://github.com/FrenchFive/mobydick/assets/105274118/074dc0bb-9473-45ac-a25b-8b1fd3d40ef6)

WHATEVER THE OPTION YOU PICKED.
<br> You should end up with the blue line. **WHICH SHOULD BE YOUR PATH**

TO CLONE YOU WILL NEED TO TYPE : 
```batch
git clone LINK
```
LINK :: The link we copied earlier

![image](https://github.com/FrenchFive/mobydick/assets/105274118/f4b2ae98-6d58-4d13-be31-5b2e085d1274)

---
YOU ARE DONE !!!
