#  Parallel coding using OpenMP 
### Different types of Matrix Multiplication
##### 1. Ordinary Matrix Multiplication (OMM).
##### 2. Block Matrix Multiplication (BMM) using block sizes: 4,8,16,32,64.
##### 3. Tranpose of A to find nth Power using OMM.
##### 4. Tranpose of A to find nth Power using BMM.
### Graphs the different types of Multiplications
##### a. Runtime vs. Matrix Sizes by fixing number of threads
##### b. Runtime vs. Threads by fixing the Matrix Size.
***
### 1. Ordinary Matrix Multiplication (OMM).
Code Description
- Initializes matrices A and B with random values.
- Allows us to specify the number of threads for parallelization.
- Uses OpenMP to parallelize the matrix multiplication.
- Measures the elapsed time for the multiplication process.
- Outputs the elapsed time in seconds.
### Graphs
a. Runtime vs. Threads by fixing the Matrix Size. (Threads varies as 1,2,4,6,8,10,12,14,16)

![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/77862e53-24eb-4837-90b0-17e61a0e0b76)

![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/ebec57f2-099c-4403-b543-4156dac43fce)

![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/4ef9b012-5307-4ae2-8d72-566f74b6d0f9)


b. Runtime vs. Matrix Sizes by fixing number of threads (Matrix Sizes - 512, 1024, 2048)
 
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/1d6aa66e-ea5c-4918-9cbd-5a8144c2579d)

![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/867f11c9-5009-424c-93ee-57dab8b1b084)

![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/47654cb2-0fc5-4d76-8910-2d889e7dc825)

![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/597a4fc8-4243-4db1-8c61-4c2131a9ac69)

![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/460757a9-980a-400f-9995-ca2b4f739b26)

![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/8503e128-595f-4d2d-aff7-28edb3aad632)

![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/4b7e1817-652b-411f-9481-5bd5f1fd7d34)

![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/08614223-fcb8-4fd7-9cf4-d0500c457bd1)
***
### 2. Block Matrix Multiplication (BMM) using block sizes: 4,8,16,32,64.
- Initialization of Matrices A and B:

We start by initializing matrices A and B with random values. This step ensures that our matrices have valid data for multiplication.
User-Defined Thread Count:

We give you the flexibility to specify the number of threads to be used for parallelization. This allows you to optimize performance based on the number of available CPU cores or other considerations.

- Parallel Matrix Multiplication with OpenMP:

The core of our implementation lies in parallelizing the matrix multiplication using OpenMP. OpenMP allows us to harness the power of multiple threads and divide the workload efficiently.
To achieve this, we break the matrix into smaller blocks and distribute these blocks among the threads for simultaneous computation.

- Exploring Block Sizes:

We understand that different block sizes can have varying impacts on performance. Therefore, our program lets you specify the block size.
Matrix multiplication is carried out by taking into account these block sizes, allowing you to experiment and analyze the effects on execution time.

- Timing the Process:

To evaluate the efficiency of our BMM implementation, we measure the elapsed time for the entire matrix multiplication process.
We utilize functions like gettimeofday() to ensure accurate timing and capture the start and end times.

- Outputting Elapsed Time:

After completing the matrix multiplication, we provide you with the elapsed time in seconds.
This information is invaluable for assessing the efficiency of our BMM algorithm under different configurations.


### Graphs
a. Runtime vs. Threads by fixing the Matrix Size. (Threads varies as 1,2,4,6,8,10,12,14,16)
- For Matrix odf size 2048 and blocks size varies as 4,8,16,32,64

 ![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/1422f67f-08dc-4947-9c07-e2f7130e7933)
 ![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/78597755-1ac1-41e7-8439-c45341b8c11d)
 ![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/75b82b8a-d341-4e67-8a46-38661eb1b667)
 ![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/2ddda011-0bb9-4443-9d9c-052da54a2e1e)
 ![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/6b0bc908-b175-496b-bb7c-322b77673dd3)

- For Matrix odf size 1024 and blocks size varies as 4,8,16,32,64
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/277a5ccd-c778-430e-ad42-cf81c06d8bb4)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/5ccd141c-7590-405b-8f25-d830d84e93e4)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/61cb1dd4-e906-4f7a-be79-e2e77316ed5b)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/1d5cf369-c610-48a6-979a-d8b1881f6dfc)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/234cbf75-aaa8-4dfc-a09f-a33abe6955a0)

- For Matrix odf size 512 and blocks size varies as 4,8,16,32,64
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/d09e819b-57a9-4339-aa94-3bbd99aae755)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/18e35ada-be8e-4721-b1ed-559d9cb9d5a8)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/cc24dbcb-59bd-4282-9643-91ab47afc680)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/ec864e26-2db5-4976-94f6-4f7091e1a26e)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/9f7c2dcd-767a-4d7f-ba51-3673787cf6e7)

b. Runtime vs. Matrix Sizes by fixing number of threads (Matrix Sizes - 512, 1024, 2048)
- in this we kept thread number as constant in each case and changed the matix sizes
  
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/d445dc77-9589-4ff7-adb9-94c6143800ac)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/9dde7469-6dde-408d-82dc-906ab8a47c65)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/1ad34a61-1447-412f-9cd2-41e4c20208bb)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/0de0cf7f-434b-48ef-a713-2e4dec9fe3c7)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/522277f1-6035-4b08-9d8e-782b4ade3e34)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/8044008c-c746-460d-bffd-e9d9943ef062)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/fa0fdc66-57e8-4bd6-bd96-11efb13f883b)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/4cf594aa-49d4-4143-a832-ab194b3c43c4)

***
### 3. Tranpose of A to find nth Power using OMM.
- Initialization of Matrix A :

We start by initializing matrices A with random values. This step ensures that our matrices have valid data for multiplication.

-User-Defined Thread Count:

We give you the flexibility to specify the number of threads to be used for parallelization. This allows you to optimize performance based on the number of available CPU cores or other considerations.

- Transpose of A
  - In the regular matrix multiplication, basically we multply row of one matrix with column of another 
    matrix, instead in this transpose approach if we transpose atleast one matrix in matrix multiplication 
    process we can directly multply row with row, this helps to reduce the run time.
  - in oue approach we varied n between 2-16 where N is exponent of Am A is the matrix with order varies 
    between 512 & 2048.
  - Here exponent implies number of times of multiplication of matrix A with itself.  

- Parallel Matrix Multiplication with OpenMP:

The core of our implementation lies in parallelizing the matrix multiplication using OpenMP. OpenMP allows us to harness the power of multiple threads and divide the workload efficiently.
To achieve this, we break the matrix into smaller blocks and distribute these blocks among the threads for simultaneous computation.

- Outputting Elapsed Time:

After completing the matrix multiplication, we provide you with the elapsed time in seconds.
This information is invaluable for assessing the efficiency of our BMM algorithm under different configurations.

### Graphs
a. Runtime vs. Threads by fixing the Matrix Size. (Threads varies as 1,2,4,6,8,10,12,14,16)

- EXPONENTS i.e, no of Matrixes being multiplied in an itreation will be from 2 to 10.
  
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/aaaea239-494f-4ccb-8820-c5f9c40ce495)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/ea49bc5a-a93f-4bf7-a3b7-469807cca734)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/2b7231b8-09b3-430b-8dcb-81780f7b23a1)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/54f506e0-88bf-4efa-886e-5c5892d16faf)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/b548f08c-0791-4d61-972c-d95965157f05)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/f5f8e581-e532-4354-ab81-63406bba8266)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/0b1b45ec-c870-4282-a0a3-1ea8fa8ec70a)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/1d2455c2-817c-4b8e-bd87-369b1a58509c)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/e3823f34-4e81-4e61-8c4d-a5c7fadf7ed0)


b. Runtime vs. Matrix Sizes by fixing number of threads (Matrix Sizes - 512, 1024, 2048)
- in this we kept thread number as constant in each case and changed the matix sizes

![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/7626a7c6-9950-4684-83b6-8fff1a626b41)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/cda27830-dc3f-4051-86c0-17a9cb8c4f9c)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/1e35f485-4da2-4f1b-b486-78df0594ff65)

![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/fa281152-3b33-4db3-ba48-531909c31642)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/7c8a749a-6ada-4339-ba80-a8c59fc96df5)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/ce2d5909-e6ee-49bf-8d81-ab71a2fd120b)

![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/58a67d9d-f938-4ad1-8b77-1b69ba65187b)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/c533ea10-59a0-4b21-9237-203623361cb6)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/f31b602d-db4a-41ae-a116-6b2e8292775b)

### 4. Tranpose of A to find nth Power using BMM.

We start by initializing matrices A with random values. This step ensures that our matrices have valid data for multiplication.
- Transpose of A
  - In the regular matrix multiplication, basically we multply row of one matrix with column of another 
    matrix, instead in this transpose approach if we transpose atleast one matrix in matrix multiplication 
    process we can directly multply row with row, this helps to reduce the run time.
  - in oue approach we varied n between 2-16 where N is exponent of Am A is the matrix with order varies 
    between 512 & 2048.
  - Here exponent implies number of times of multiplication of matrix A with itself.
 
- Exploring Block Sizes:

We understand that different block sizes can have varying impacts on performance. Therefore, our program lets you specify the block size.
Matrix multiplication is carried out by taking into account these block sizes, allowing you to experiment and analyze the effects on execution time.

- Timing the Process:

To evaluate the efficiency of our BMM implementation, we measure the elapsed time for the entire matrix multiplication process.
We utilize functions like gettimeofday() to ensure accurate timing and capture the start and end times.

- Outputting Elapsed Time:

After completing the matrix multiplication, we provide you with the elapsed time in seconds.
This information is invaluable for assessing the efficiency of our BMM algorithm under different configurations.


### Graphs
a. Runtime vs. Threads by fixing the Matrix Size. (Threads varies as 1,2,4,6,8,10,12,14,16)
- For Matrix odf size 2048 and blocks size varies as 4,8,16,32,64
  
EXPONENT - 2 & MATRIX SIZE - 2028

![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/f56ff4e3-3fe5-4ceb-918f-1e7007908d36)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/bed55461-27ed-4cfc-bb33-1d6ecc7dd4bb)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/6042b3b2-b7d1-4675-9e5c-f096fcad41f0)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/e2f87633-e301-408e-bf00-11d2e62ad600)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/550ae726-76c8-4c7d-8e68-713e4cd4be42)

EXPONENT - 2 & MATRIX SIZE - 1024

![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/66590d0b-a253-4338-bd98-fd21c37aa880)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/052bb4cb-32a5-493b-b518-88920575ba16)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/34a60a66-c058-40c6-9203-0dfe1b5b7352)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/fa0679ba-b455-47e9-9932-d1ca8c72223b)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/40730e48-d964-4820-bd77-21fb1fd4745d)

EXPONENT - 2 & MATRIX SIZE - 512

![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/0cd732fd-2093-41af-bb3a-e1f7b0c4adbe)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/85ec8e29-2218-48f0-a0fb-b6fb3d7a3be2)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/d9dd5153-6cff-457f-b86a-37c8086943c7)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/4d08e949-1985-4bb2-8bc9-1c57bf9f7894)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/662934b4-be01-4eb2-ac26-58fcabf505b7)

EXPONENT - 8 & MATRIX SIZE - 512

![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/341ea1f7-43d0-4eda-9e64-11d7a47fa4ea)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/c2152df6-b9d3-4769-ac32-4182d8f9bf51)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/ceb805e3-efbb-4eff-82c5-6b6b32fd549a)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/ea84b3c3-3a28-4bbb-8e4f-1d6016c778d4)

EXPONENT - 8 & MATRIX SIZE - 1024

![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/87b792a1-1760-4a2a-9e8f-c93744717013)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/5e9e1a2e-0a2f-4ea2-9f99-e4f0ed834105)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/0b7865ac-7c39-43cb-b5c3-46acf1508e8f)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/13d2ec77-8e0c-4b72-8d15-1a7818da472c)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/7c1873d4-e09f-488e-a06c-e51f9641ff9a)

EXPONENT - 8 & MATRIX SIZE - 2048

![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/6840c506-ce62-4310-a5e4-7aee0ab1f548)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/8cf20c33-02e5-43f7-8f21-81bdf35c1814)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/c835c586-be55-4283-9f5b-c4413ba63e99)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/6ba4f24d-a67b-4e2a-8cb4-809e04bd9e20)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/14b75724-837a-4aa7-a71c-be90649f4f24)

b. Runtime vs. Matrix Sizes by fixing number of threads (Matrix Sizes - 512, 1024, 2048)
- in this we kept thread number as constant in each case and changed the matix sizes
- Block size varies between 4,16,32
  

Threads constant as 8
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/a969806d-7d71-481b-a837-b8c51ab84163)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/ef154154-83bf-4af3-96a9-7a3741243622)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/68174da5-a76f-4e63-9f44-a67ad78c6bdf)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/b0ef43d6-dee8-4453-844e-e7fe709b2054)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/632ff709-45d2-4997-b29e-4d29ea6419cf)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/a0cb81fd-e3ea-4713-93e7-00c708e54f41)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/86beb2e1-eec4-4caf-bf9b-11b593c02f08)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/15b2a184-8171-4baa-b189-72a7e3a4740f)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/53de4e67-0709-4643-8c2d-b3712d9c265b)


Threads constant as 16
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/000ab674-17e6-4863-a549-f0bd3f9a2c12)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/b03c93d1-0835-4b49-aff5-5847309d9979)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/beffce8d-f0c4-4de1-a5ed-33e259cc1060)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/213aa67d-d29b-4e10-8b6e-803d5f647d83)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/ca7f6f7d-3566-4dbb-9183-f818b7de9a61)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/50136911-daf2-43ec-98dc-95893e73063b)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/72ca32c9-2d34-416b-8d2a-cd38768c1e67)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/9638bbde-b4f0-49d5-ab14-e0fca3f2f928)
![image](https://github.com/chaitanyabalajireddy/HPC_Assignment-_1/assets/91625648/689a4acf-81b5-4e7c-88c3-b30c324270fe)


