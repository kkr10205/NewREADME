# NewREADME
### Shell Script to  parse the attached log file
>Blockquote
```
#!/bin/bash
for i in *zip
do
echo "removing already exists log file" 
rm *log
echo "unzip the zip file"
unzip $i
echo ".............................."
echo disply the log file
cat *log                                                                    
echo "............................."
echo "Display the command line argument "
echo $1
done
```
#### Explanation of the script
- At first we use the for loop to get the file
- Inside for loop we first remove the log file which is already exist outside the zip file using rm command
- Then we unzip the zip file using unzip command
- After that we use cat command to display the unziped log file
-Then using $1 we display the result for commnad line argument
