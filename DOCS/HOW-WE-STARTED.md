We started with such script
```bash
#!/bin/bash
## EXAMPLE:
# sh readme.sh
## CONFIG:
FILE_LIST=".readme.txt"
FILE_OUTPUT="README.md"
CONTENT_LIST=$(cat $FILE_LIST)
# START:
echo "<!-- START: This file is rendered, dont' edit it, just separated parts --> " > $FILE_OUTPUT
for content_file in $CONTENT_LIST
do
echo $content_file
if [ -f $content_file ]
then
echo "<!-- $content_file --> " >> $FILE_OUTPUT
cat $content_file >> $FILE_OUTPUT
fi
done
echo "<!-- END: This file is rendered, dont' edit it, just separated parts --> " >> $FILE_OUTPUT
# END
## TEST readme.md
cat README.md
firefox README.md
```
