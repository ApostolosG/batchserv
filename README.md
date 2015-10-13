#batchserv
#!/usr/bin/env bash
#Script for  HRIT data batch interpretation

DIR=/home/tollis/input/
LIR=/home/tollis/xuma/
TMP=/home/tollis/trash/

#mpeno sto fakelo

cd $LIR
for i in  $LIR/*;
do

cp $i $DIR

hritseven $DIR

cd $DIR

for k in  $DIR/*;

do

#metakino ta arxeia
mv $k $TMP

done
done
