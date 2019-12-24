## commands to run 1.12

```diff
+/Docker/part1/1.12$ docker run -d -p 5000:5000 frontend
286d6200a3be7980d49f90f5280b3ac5503b8ad49e008f6450b0855ab0e5036f
+/Docker/part1/1.12$ docker run -d -p 8000:8000 -v $(pwd)/logs.txt:/backend-example-docker/logs.txt backend
f5095e1cfff7f5879fcf32ce512b78be92131c06a805c318419b1ce3a8cb3c37
+/Docker/part1/1.12$ docker ps
CONTAINER ID        IMAGE               COMMAND             CREATED             STATUS              PORTS                    NAMES
f5095e1cfff7        backend             "npm start"         4 seconds ago       Up 2 seconds        0.0.0.0:8000->8000/tcp   xenodochial_moore
286d6200a3be        frontend            "npm start"         45 seconds ago      Up 44 seconds       0.0.0.0:5000->5000/tcp   frosty_villani
+/Docker/part1/1.12$ cat logs.txt 
12/24/2019, 8:02:00 AM: Connection received in root
12/24/2019, 8:02:02 AM: Connection received in root
+/Docker/part1/1.12$
```
