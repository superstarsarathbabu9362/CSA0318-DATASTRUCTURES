

#include <stdio.h>

int main()

{

   int arr[100], key, i, no, count = 0, search;

   printf("Enter number of elements you would like to take as input\n");

   scanf("%d", &no);

   printf("Enter %d numbers\n", no);

   for (i= 0; i < no; i++)

      scanf("%d", &arr[i]);  

   printf("Enter a number that you would like to search\n");

   scanf("%d", &search);  

   for (i = 0; i < no; i++) {

      if (arr[i] == search) {

         printf("%d is present at position %d.\n", search, i+1);

         count++;

      }

   }

   if (count == 0)

      printf("%d key is not present in the array.\n", search);

   else

      printf("%d is present %d times in the array.\n", search, count);    

   return 0;

}
