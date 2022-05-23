![file](file.png)

- `FROM` : make basic image.FROM is a **required** command and must be the **first** command.
- `RUN` : Used to execute command line commands.There are two formats:
  -  shell format: `RUN <command>`
  -  exec format: `RUN ["executable", "parameter 1", "parameter 2"]`
    The default permission for the **run** command is **sudo**, which adds a **new layer** to the docker **each time** run is executed.
- `COPY` : 
