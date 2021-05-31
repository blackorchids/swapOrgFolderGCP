#!/bin/bash

ls $PWD/inventory > $PWD/temp
i=0 
while IFS= read -r line
do
   #echo $line
   i=0
   while IFS= read -r subfolder_line
   do
     #echo $subfolder_line
     arrs[$i]=$subfolder_line
     #echo $i
     ((i=i+1))
   done < $PWD/inventory/$line
   #echo ${arrs[4]}
   #echo ${#arrs[*]}  length of arrays
   #echo ${arrs[-1]}  print last element
   org=""
   for (( x=${#arrs[*]}; x>1; x-- ))
   do
	org+=${arrs[$x-1]}/
   done
   
   echo ${arrs[0]},$org 

done < $PWD/temp

#rm -rf $PWD/temp
