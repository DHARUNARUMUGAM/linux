# linux

FIBONACCI SERIES:

!/bin/bash
echo "enter"
read n
a=0
b=1
for ((i=0;i<n;i++))
{
   echo -n "$a "
   fn=$((a+b))
   a=$b
   b=$fn
}

FACTORIAL:

echo "enter a number"                                                                         
read n                                                                                        
x=1                                                                                           
for((i=2;i<=n;i++))                                                                           
{                                                                                             
    x=$((x*i))                                                                                
}                                                                                             
echo $x

FIND THE LARGEST NUMBER:

#!/bin/bash
echo "enter number1:"
read a
echo "Enter number2:"
read b
echo "Enter Number3:"
read c
if [ $a -gt $b ] && [ $a -gt $c ]
then
echo $a
elif [ $b -gt $a ] && [ $b -gt $c ]
then
echo $b
else
echo $c
fi

SUM OF THE NUMBERS:

#! bin/bash
echo "Sum of N numbers"
echo "Enter a Number:"
read n
sum=0
for ((i=0;i<=n;i++))
do
    sum=$((sum+i))
done
echo "Sum of Numbers is"$sum

ARITHMATIC OPERATIONS:

#!/bin/bash
read n
read a
read b
if [ $n == 1 ]
then
c=`expr $a + $b`
echo "$a + $b = $c"
elif [ $n == 2 ]
then
c=`expr $a - $b`
echo "$a - $b = $c"
elif [ $n == 3 ]
then
c=`expr $a \* $b`
echo "$a \* $b = $c"
elif [ $n == 4 ]
then
c=`expr $a / $b`
echo "$a / $b = $c"
fi
