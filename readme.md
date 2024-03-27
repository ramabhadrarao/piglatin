Below are some common Hadoop Distributed File System (HDFS) commands that you can use in the terminal:

1. **List files/directories**:
   - Command:
     ```bash
     hdfs dfs -ls /path/to/directory
     ```
   - Description:
     This command lists all files and directories present in the specified HDFS directory.

2. **Create a directory**:
   - Command:
     ```bash
     hdfs dfs -mkdir /path/to/new_directory
     ```
   - Description:
     This command creates a new directory in the specified HDFS path.

3. **Copy files/directories from local file system to HDFS**:
   - Command:
     ```bash
     hdfs dfs -copyFromLocal /path/to/local_file_or_directory /path/to/hdfs_destination
     ```
   - Description:
     This command copies files or directories from the local file system to the specified HDFS destination.

4. **Copy files/directories from HDFS to local file system**:
   - Command:
     ```bash
     hdfs dfs -copyToLocal /path/to/hdfs_file_or_directory /path/to/local_destination
     ```
   - Description:
     This command copies files or directories from the specified HDFS location to the local file system.

5. **Move files/directories within HDFS**:
   - Command:
     ```bash
     hdfs dfs -mv /path/to/source /path/to/destination
     ```
   - Description:
     This command moves files or directories from the source path to the destination path within HDFS.

6. **Remove files/directories from HDFS**:
   - Command:
     ```bash
     hdfs dfs -rm /path/to/file_or_directory
     ```
   - Description:
     This command removes the specified file or directory from HDFS.

7. **View the contents of a file**:
   - Command:
     ```bash
     hdfs dfs -cat /path/to/file
     ```
   - Description:
     This command displays the contents of the specified file in HDFS.

8. **Change permissions of a file/directory**:
   - Command:
     ```bash
     hdfs dfs -chmod <permissions> /path/to/file_or_directory
     ```
   - Description:
     This command changes the permissions of the specified file or directory in HDFS.

9. **Change ownership of a file/directory**:
   - Command:
     ```bash
     hdfs dfs -chown <user>:<group> /path/to/file_or_directory
     ```
   - Description:
     This command changes the ownership of the specified file or directory in HDFS.

10. **Check disk usage of files/directories**:
    - Command:
      ```bash
      hdfs dfs -du -h /path/to/file_or_directory
      ```
    - Description:
      This command displays the disk usage of the specified file or directory in HDFS in a human-readable format.
