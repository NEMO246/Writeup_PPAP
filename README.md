# Writeup_PPAP

![image](https://github.com/user-attachments/assets/6df20bc2-b02f-4332-82ee-19e0decfe56d)

![image](https://github.com/user-attachments/assets/fc905650-93a0-4e7d-8947-c8d3b0472ed0)

With the condition of the task (In Japan, we send attachments, we set a password and send the password by separate mail), we understand that we need to search for a message with a file and a password.
To do this, we can search by the data-text-lines filter.

![image](https://github.com/user-attachments/assets/b5319c28-da13-44db-99fa-f36e35a5f61e)

We find two messages sent by the SMTP protocol.
(https://uk.wikipedia.org/wiki/SMTP)
![image](https://github.com/user-attachments/assets/b02a2af2-8a1e-4b5e-a3eb-9ae12340a050)

We are reviewing the content of the messages.
![image](https://github.com/user-attachments/assets/be878ab3-2870-4301-9830-29fde2177f12)

In the first message, we can see the name of the archive and the archive itself in Base64 format.
![image](https://github.com/user-attachments/assets/61b8466f-3933-45d2-adc3-e42fdb4d4a2c)
![image](https://github.com/user-attachments/assets/9bbbdd90-ff83-4f8b-85d8-5d14ce6f8efa)

To decode the archive, we can make a small script, insert the entire base64 from the message into base64_string.
![image](https://github.com/user-attachments/assets/5b4dd99f-4163-48b4-8d47-5dc1905968a5)

After running the script, we will create an archive in which there will be a folder containing a document that needs a password.
![image](https://github.com/user-attachments/assets/ecb41f70-a3b0-4e31-ac6b-a41310c90257)

Now let's return to the second message in which we will find the password for the document.
![image](https://github.com/user-attachments/assets/53357153-45e2-4dec-95bd-73a984158a60)

We will use the document with the password bS9K5vGz and get a flag
![image](https://github.com/user-attachments/assets/cc686ba2-07d1-4bdb-8904-742dc4838df8)

FLAG: no_more_PPAP

