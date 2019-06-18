# Raspberry-Face-Recognition
Real-time face recognition project with opencv. It works on Raspberry Pi 3 B+ OS.

**01_face_dataset.py**：Automatically detect face and gather images into dataset.  

**02_face_training.py**：Train the model to make it recognize users in dataset. Encryption password is required to ensure security for     trained *yml* file. The md5 value of password acts as encryption key of AES-CBC process. Redundancy backup file is generated to guarantee integrity, since the system works on embedded environment.  

**03_face_recognition.py**: Recognition process. Check consistency between trained model and backup model. Use password's md5 to decrypt *yml* file. If wrong, an error message would be given.

**Result preview:**
![avatar](http://b.hiphotos.baidu.com/image/pic/item/32fa828ba61ea8d3fcd2e9ce9e0a304e241f5803.jpg)
