Below are some common Hadoop Distributed File System (HDFS) commands that you can use in the terminal:

1. **List files/directories**:
   ```bash
   hdfs dfs -ls /path/to/directory
   ```

2. **Create a directory**:
   ```bash
   hdfs dfs -mkdir /path/to/new_directory
   ```

3. **Copy files/directories from local file system to HDFS**:
   ```bash
   hdfs dfs -copyFromLocal /path/to/local_file_or_directory /path/to/hdfs_destination
   ```

4. **Copy files/directories from HDFS to local file system**:
   ```bash
   hdfs dfs -copyToLocal /path/to/hdfs_file_or_directory /path/to/local_destination
   ```

5. **Move files/directories within HDFS**:
   ```bash
   hdfs dfs -mv /path/to/source /path/to/destination
   ```

6. **Remove files/directories from HDFS**:
   ```bash
   hdfs dfs -rm /path/to/file_or_directory
   ```

7. **View the contents of a file**:
   ```bash
   hdfs dfs -cat /path/to/file
   ```

8. **Change permissions of a file/directory**:
   ```bash
   hdfs dfs -chmod <permissions> /path/to/file_or_directory
   ```

9. **Change ownership of a file/directory**:
   ```bash
   hdfs dfs -chown <user>:<group> /path/to/file_or_directory
   ```

10. **Check disk usage of files/directories**:
    ```bash
    hdfs dfs -du -h /path/to/file_or_directory
