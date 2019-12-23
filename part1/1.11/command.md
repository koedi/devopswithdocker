## Used command
```diff
+ Docker/part1/1.11$ docker run -v $(pwd)/logs.txt:/backend-example-docker/logs.txt -p 8000:8000 backend
```

## log output
```diff
+ Docker/part1/1.11$ cat logs.txt 
12/23/2019, 7:40:09 AM: Connection received in root
12/23/2019, 7:40:12 AM: Connection received in root
12/23/2019, 7:40:12 AM: Connection received in root
12/23/2019, 7:40:12 AM: Connection received in root
```

