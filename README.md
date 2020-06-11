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
