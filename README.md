# STDSR_Assignment_2
Assignment 2 task 2 code

All code are within one file ```STDSR_Assignment_2_Task_2.ipynb```. To use the code additional libraries ```geojson```, ```descartes``` and ```geopy``` is needed. Also need [city.csv](https://github.com/hflabs/city) file with russia cities information and [russia.json](https://www.dropbox.com/s/sadvwkzbqjjurdv/russia.json?dl=1) file with geojson format of russia borders.

## Slow cooling
Here i used SA with T0=400, T_cool=20 and T_decrease_rate=0.999. Temperature decreased every 2nd iteration. For a total of 6000 iterations SA found optimal distance 22k km. For a video every 10 iteration were used


https://user-images.githubusercontent.com/69848346/235898081-b0758b3a-00ba-4d27-9958-afa621a6d2aa.mp4


## Middle cooling
Here i used SA with T0=2000, T_cool=20 and T_decrease_rate=0.99. Temperature decreased every 2nd iteration. For a total of 700 iterations SA found optimal distance 23k km.


https://user-images.githubusercontent.com/69848346/235898107-e096fcdb-01b0-4e5a-aaeb-1b716222a9e0.mp4


## Fast cooling
Here i used SA with T0=40000, T_cool=20 and T_decrease_rate=0.95. Temperature decreased every 2nd iteration. For a total of 300 iterations SA found optimal distance 28k km.


https://user-images.githubusercontent.com/69848346/235898114-3c7bf053-61c1-4cc0-92fb-7dee08c2f67d.mp4


In total, slow cooling showed the best performance out of all, but this may be because of total number of iterations. To resolve this problem i may inrease initial temperature, but this affects on acceptance ratio and showed to be not useful. Increasing number of iterations to cool down also didn't show much effect. Middle cooling showed similar result in distance, but with 10x more speed, which may be useful in some cases.
