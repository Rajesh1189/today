#!/bin/bash
echo " ENTER THE WORD"
read WORD
grep -l -R "$WORD" *> temp_file.txt
if [ $? -eq 0 ];
then
echo "$WORD IS FOUND IN BELOW FILES"
cat temp_file.txt
else
echo "PATTEREN NOT FOUND"
fi
