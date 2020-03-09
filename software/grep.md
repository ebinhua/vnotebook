# grep

echo who am i | grep -q "^Kenny$"

if [ $? -ne 0 ] ;then

   echo "grep return a none-zero value, not find Kenny"

else

   echo "grep return zero value, find Kenny"

fi
