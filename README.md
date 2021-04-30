# Voxel Engine Project
### Goal:
to create a 3D voxel rendering engine from scratch that could render 10^8 – 10^9 voxels on screen at once, modifiable in real time and rendered at interactive frame rates.

### Challenges: 
There were dozens of challenges with this project, one salient one was to realize the traditional computer graphics rendering pipeline was fundamentally ill-suited for this task. This required me to learn modern GPGPU methods to even begin working on the project. From there, many problems arose due to multithreaded memory writes/reads (There can be thousands of threads per dispatch). This was  resolved by reworking algorithms to work with built in functions that managed memory accesses in an atomic way. 
This project took months to realize and intense mental effort every step of the way. 

![shadow monster](https://user-images.githubusercontent.com/22987416/116649695-c09f7000-a934-11eb-90d1-530c237701cf.jpg)
![translucency](https://user-images.githubusercontent.com/22987416/116649717-cb5a0500-a934-11eb-9152-ac3549806f96.jpg)
![come on](https://user-images.githubusercontent.com/22987416/116727970-2540e600-a99a-11eb-9e55-05d42b1dfd86.jpg)
