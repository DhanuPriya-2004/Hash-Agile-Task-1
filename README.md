# Hash-Agile-Task-1

Sample code 1:
find_second_largest() {
 if [ ${#arr[@]} -lt 2 ]; then
 echo "Array should contain at least two elements."
 return
 fi
 largest=-2147483648
 second_largest=-2147483648 
 for num in "${arr[@]}"; do
 if (( num > largest )); then
 second_largest=$largest
 largest=$num
 elif (( num > second_largest )) && (( num != largest )); then
 second_largest=$num
 fi
 done 
 if (( second_largest == -2147483648 )); then
 echo "No second largest element found."
 else
 echo "Second largest element is: $second_largest"
 fi
}
arr=(24 23 13 31 4)
find_second_largest
sample output 1:
output:
seconf largest element is : 24
Sample code 2:
find_second_largest() {
 if [ ${#arr[@]} -lt 2 ]; then
 echo "Array should contain at least two elements."
 return
 fi
 largest=-2147483648
 second_largest=-2147483648 
 for num in "${arr[@]}"; do
 if (( num > largest )); then
 second_largest=$largest
 largest=$num
 elif (( num > second_largest )) && (( num != largest )); then
 second_largest=$num
 fi
 done 
 if (( second_largest == -2147483648 )); then
 echo "No second largest element found."
 else
 echo "Second largest element is: $second_largest"
 fi
}
arr=(10 23 89 5 43 )
find_second_largest
sample output 2:
output:
seconf largest element is : 43
Sample code 3:
find_second_largest() {
 if [ ${#arr[@]} -lt 2 ]; then
 echo "Array should contain at least two elements."
 return
 fi
 largest=-2147483648
 second_largest=-2147483648 
 for num in "${arr[@]}"; do
 if (( num > largest )); then
 second_largest=$largest
 largest=$num
 elif (( num > second_largest )) && (( num != largest )); then
 second_largest=$num
 fi
 done 
 if (( second_largest == -2147483648 )); then
 echo "No second largest element found."
 else
 echo "Second largest element is: $second_largest"
 fi
}
arr=(44 78 54 23 12 )
find_second_largest
sample output 3:
output:
seconf largest element is : 54
