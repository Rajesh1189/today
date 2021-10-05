#! /bin/bash
if [ $# -ne 3 ];
then
echo " PASS ONLY THREE ARGS "
exit
fi
if [ $1 -lt $2 ] && [ $1 -lt $3 ]
then
echo " $1 IS SMALL "
elif [ $2 -lt $1 ] && [ $2 -lt $3 ];
then
echo " $2 IS SMALL "
else
echo " $3 IS SMALL "
fi
