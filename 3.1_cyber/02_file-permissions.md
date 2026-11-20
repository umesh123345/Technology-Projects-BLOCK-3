# Understanding File Permissions

## Task 1 --- Create a File

Run:

    touch secret.txt
    ls -l secret.txt

### Screenshot
<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/22420ebc-9f7a-44f1-992f-2463db2bf32a" />



### Questions

1.  Who owns the file?
2.  
3.  What are the default permissions?

### Reflection

Why is file ownership important in Linux systems?

------------------------------------------------------------------------

## Task 2 --- Restrict File Permissions

Run:

    <img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/44cbf3d5-04e2-47d6-956f-8ab6495cec88" />


### Screenshot
<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/56defa78-c9ce-4485-8212-b4992f836306" />


### Questions

1.  Who can read the file now?
2.  Who cannot access it?


------------------------------------------------------------------------

## Task 3 --- Open Permissions (Security Risk)

Run:

    chmod 777 secret.txt
    ls -l secret.txt

### Screenshot
<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/eba0423e-2b33-46b1-953c-477f125ed187" />


### Questions

1.  Who can access the file now?
2.  Why might this configuration be dangerous?

