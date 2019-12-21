## Command to run container

```diff
+kpietika@lx9-fuxi195:~/Documents/Opinnot/Docker/part1/1.8$ docker run -v $(pwd)/logs.txt:/usr/app/logs.txt devopsdockeruh/first_volume_exercise
(node:1) ExperimentalWarning: The fs.promises API is experimental
Wrote to file /usr/app/logs.txt
^CClosing file
+kpietika@lx9-fuxi195:~/Documents/Opinnot/Docker/part1/1.8$ ls
logs.txt
+kpietika@lx9-fuxi195:~/Documents/Opinnot/Docker/part1/1.8$ cat logs.txt 
Sat, 21 Dec 2019 08:43:43 GMT
+kpietika@lx9-fuxi195:~/Documents/Opinnot/Docker/part1/1.8$ 
```
