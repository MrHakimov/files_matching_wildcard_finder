# files-matching-wildcard-finder
Write command line application which executes a recursive search for files matching specified wildcard pattern in the specified directories. This application should work on macOS/Linux/Windows.

Example:

```
> java -jar myjar.jar -dir /dir1  -dir /dir2 -pattern "*.{so,md}"
Let we have the following files structure:

/dir1/app/app
/dir1/app/app.yml
/dir1/app/howtouse.md
/dir1/app/data.bin
/dir1/app/libs/arm64-v8a/library-2.11.1.so
/dir1/app/libs/x86/library-2.11.1.so
/dir2/docs/list.json
/dir2/docs/readme.md
/dir2/docs/tutorial/part1.md
```
This application should return the following file paths in stdout:

```
/dir1/app/howtouse.md
/dir1/app/libs/arm64-v8a/library-2.11.1.so
/dir1/app/libs/x86/library-2.11.1.so
/dir2/docs/readme.md
/dir2/docs/tutorial/part1.md
```
Hint: To find files could be used glob matcher from standard Java NIO library.

Provide the application code or link to the public code repository and description of how to use it.

**The solution of the problem is given in this repository.**
***
### How to use?
1. Download [FilesMatchingWildcardRegularExpression.jar](out/artifacts/FilesMatchingWildcardRegularExpression_jar/FilesMatchingWildcardRegularExpression.jar);
2. Mark the file in the folder with the files and directories that you want to work;
3. Run file on the command line.

*_To search for files in the folder where the jar-archive is located, simply add to arguments "-dir /" or "-dir //"_
***
### Example
1. All my neccessar directories and files are in folder "x":
![screenshot of folder "x"](media/002.PNG)
2. Running file on the command line:
![screenshot of command line](media/001.PNG)
