# archiv - A directory archiver
This is a simple utility designed to archive a specified directory into a timestamped .tar.gz archive file. This could be used to archive any directory in an organized fashion.

### Prerequisites
- A Unix-like system (Linux or macOS) with Bash installed.
- The tar command (usually pre-installed on Unix-like systems).

### Usage
To run this script, you need to pass the directory you want to archive as an argument. The script will:

- Check if an argument is provided.
- Check if the argument is a valid directory.
- Create a timestamped archive of the directory if valid.
- Store the archive in a subdirectory named archives.

```
./directory_archiver.sh <directory_path>
```

#### Example
```
./directory_archiver.sh /path/to/my_directory
```

If successful, the script will create an archive named something like `logs_archive_20250217_152530.tar.gz`.

### Notes
- The script creates the `archives` directory in the current working directory if it doesn't exist.
- The timestamp format for the archive name is `YYYYMMDD_HHMMSS`, based on the current date and time e.g. `20250416_124038`.
- The archive is compressed using gzip (i.e., .tar.gz format).

### License
This script is released under the ISC License.