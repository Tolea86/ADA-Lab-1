# ADA-Lab-1
ADA Laboratory Work Nr.1 st.gr. TI-191M Iuzvac Anatolie

## Executed Work

1. Compiled proposed code, executed app with sleepy and busy parameters and logged the execution times on my machine.

    **Sleepy** execution time - 12.642 seconds

    **Busy** execution time - 15.895 seconds

2. Created lab1_openmp.c and parallelized the execution of **sleepy_fibonacci** and **busy_fibonacci** usin **OpenMP**, logged times for proposed thread numbers : 

| Număr fire        | 1           |   2    |   4    |    8   |    16  |   32   |
| ----------------- |-------------| ------ | ------ | ------ | ------ | ------ |
| Sleepy            | 12.603s     | 6.317s | 3.281s | 1.754s | 1.030s | 0.525s |
| Busy              | 15.956s     | 7.928s | 4.438s | 4.381s | 4.304s | 4.273s |

3. Created lab1_openmpi.c and parallelized the execution of **sleepy_fibonacci** and **busy_fibonacci** usin **OpenMPI**, logged times for proposed thread numbers : 

| Număr fire        | 1           |   2    |   4    |    8   |    16  |   32    |
| ----------------- |-------------| ------ | ------ | ------ | ------ | ------- |
| Sleepy            | 12.725s     | 6.449s | 3.725s | 2.296s | 1.738s | 5.874s  |
| Busy              | 16.256s     | 8.159s | 4.704s | 4.876s | 5.383s | 14.759s |

4. 

a) The utility of used libraries **OpenMP** and **OpenMPI** is enormous in parallelizing codes in order to increase time-efficiency of the application. As from our current experience can make a comparison between **OpenMP** and **OpenMPI**, the main difference between these two libraries is that **OpenMPI** runs different instances of the same app which should communicate between them in order to achieve wanted result, in comparison **OpenMP** runs threads in the same app, on specific processes.

b) Analyzing the given time tables in point **2** and **3** can be observed that for **OpenMP** the number of threads does increase the time efficiency of the application, for **busy** mode there is a limit at which every process is busy and can't minimize further. For **OpenMPI** exists limitation in maximum efficient threads as there is condition that these separate threads should communicate between them which creates a waiting time of response between threads. **Amdahl's Law** states that the speedup of the process is limited at 20 times the single thread performance, which is very clearly shown in the time tables that the maximum speedup time is around 20 times the single thread performance.

