#/bin/bash

sed '1d' $1 >temp

while read line
  do
  AGE=`echo "$line" | awk -F " " '{print $3}'`
if [ $age -gt $2 ];
then
  echo $line | awk -F " " '{print $2}'
fi
done < temp
rm temp
