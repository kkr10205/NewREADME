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
