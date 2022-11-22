# Computer-Vision-based-Attendence-System

You can access the documentation here: https://studentprojectshub.blogspot.com/2021/01/computer-vision-based-attendance.html                                                                            
Data: Uploaded the data in the Repository          

[](All-Computer-Vision-Projects-with-ML-DL/blob/main/Computer%20Vision%20based%20Attendence%20System/attendence_210419.mp4)

https://user-images.githubusercontent.com/60067496/115334867-c620eb80-a1b9-11eb-93d0-5ff04b76f36e.mp4

1) HOG Feature Estimation
![image](https://user-images.githubusercontent.com/60067496/203234645-e9076b73-48bb-4d93-bc71-7df464444e69.png)
![image](https://user-images.githubusercontent.com/60067496/203234675-925a79b0-d217-4d37-b949-b47fbe873188.png)

2) Facae landmark estimation

![image](https://user-images.githubusercontent.com/60067496/203234782-597c74d7-f2db-4ac1-9de5-da829bbeabfe.png)

The basic idea is we will come up with 68 specific points (called landmarks) that exist on every face — the top of the chin, the outside edge of each eye, the inner edge of each eyebrow, etc. Then we will train a machine learning algorithm to be able to find these 68 specific points on any face

3) Face Encodings
OpenFace already did this and they published several trained networks which we can directly use. Thanks Brandon Amos and team!

So all we need to do ourselves is run our face images through their pre-trained network to get the 128 measurements for each face. Here’s the measurements for our test image

![image](https://user-images.githubusercontent.com/60067496/203235181-106440f0-d53a-43d9-96c8-95f62371cdec.png)

4) Find persons name from encoding
