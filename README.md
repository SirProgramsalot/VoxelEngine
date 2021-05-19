

# Voxel Engine Project
### Goal:
to create a 3D voxel rendering engine from scratch that could render 10^8 – 10^9 voxels on screen at once, modifiable in real time and rendered at interactive frame rates.

### Challenges: 
There were dozens of challenges with this project, one salient one was to realize the traditional computer graphics rendering pipeline wasn't the best approach for this task. This required me to learn modern GPGPU methods. From there, many problems arose due to multithreaded memory writes/reads (There can be thousands of threads per dispatch). This was  resolved by reworking algorithms to work with built in functions that managed memory accesses in an atomic way.

An important aspect of this project was getting very familiar with GPU architecture and an obssession with optimization.

### Results:
I achieved what I set out to do. Though, I did become familiar with the downsides of voxels. O(n^3) spatial complexity made certain operations very expensive (i.e. animation).

Sculpting with voxels is incredibly difficult! Below shows a variety of shaders on a variety of sculptures.

![human](https://user-images.githubusercontent.com/22987416/118868629-4316b200-b899-11eb-96f0-c708f955f9b2.jpg)
![shadow monster](https://user-images.githubusercontent.com/22987416/116649695-c09f7000-a934-11eb-90d1-530c237701cf.jpg)
![translucency](https://user-images.githubusercontent.com/22987416/116649717-cb5a0500-a934-11eb-9152-ac3549806f96.jpg)
![amaze](https://user-images.githubusercontent.com/22987416/118867913-74db4900-b898-11eb-8c3b-1124c472e6a4.jpg)
![frost demon](https://user-images.githubusercontent.com/22987416/118868198-c257b600-b898-11eb-8b9e-db1dab55b765.jpg)
