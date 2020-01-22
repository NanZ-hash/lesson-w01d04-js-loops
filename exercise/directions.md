

# Exercises: JavaScript loops

Paste your answers into this file.

<br>

## Print every number from 0 to 10

```
for ( i=0 ; i<=10 ; i++ )
{ 
  console.log(i);
}
```

<br>

## Print every number from 10 to 0

```
for ( i=10 ; i>=10 ; i-- )
{ 
  console.log(i);
}
```

<br>

## Print every number from 4 to -16

```
for ( i=4 ; i>=-16 ; i-- )
{ 
  console.log(i);
}
```

<br>

## Print every fifth number from 8 to 41

```
for ( i=8 ; i<=41 ; i+=5 )
{ 
  console.log(i);
}
```

<br>

# Exercises: JavaScript loops with array:

Paste your answers into this file.



1. Change all **odd** numbers to be those numbers multiplied by two:
```js
const numbers = [4, 9, 7, 2, 1, 8];

  const numbers = [4, 9, 7, 2, 1, 8];
let l =(numbers.length)-1;
for (i=0; i<=l ;i++)
{ 
    if (numbers[i]%2 === 0) {
        
        numbers.push (numbers[i]);
       numbers.pop();
    }
        else {
            
            numbers[i]=numbers[i]*numbers[i];
            numbers.push(numbers[i]);
            numbers.pop();
        }
}

numbers; // => [4, 18, 14, 2, 2, 8]
```

2.  Create an array to hold your favorite colors.  For each choice, log to the screen a string like: `My #1 choice is blue.`

3.  Create an array of ages.  Loop through and log only the ages that are over 21.

1. Create an array to hold your top five choices of something (music, books, movies, whatever).

    - For each choice, log to the screen a string like: "My #1 choice is blue."
    - **Bonus:** Change it to log "My 1st choice, "My 2nd choice", "My 3rd choice", picking the right suffix for the number based on what it is.

 
let colors =[]; 
colors.push('blue');
colors.push('blue');
colors.push('blue');
colors.push('blue');
colors.push('blue'); 
length=colors.length();
for (i=0; i<=length ;i++ )
{ 
   
console.log('My #'+(i+1) +'choice is'+ colors[i]);

}



## The classic Fizzbuzz Program

For every `number` between 1 and 100...

If the `number` is evenly divisible by 3, print "Fizz"

If the `number` is evenly divisible by 5, print "Buzz"

If the `number` is evenly divisible by 3 AND evenly divisible by 5, print "Fizzbuzz"


```
for ( let i=0 ; i<=100 ; i++) 
 {
 
     if (i%3 === 0 && i%5 === 0)
     
         console.log("\n FuzzBuzz");
         else if ( i%3 === 0 ) 
         console.log("\n Fuzz");
         else if ( i%5 === 0)
         console.log("\n Buzz");
     
     
     else 
     console.log("\n "+i);
 }

```

<br>


## The even/odd reporter

Write a for loop that will iterate from 0 to 20. For each iteration, it will check if the current number is even or odd, and report that to the screen (e.g. "2 is even").

```

for (let i=0 ; i< 20 ; i++)
 {  
if(i % 2 === 0)
    console.log(i+" is even ");
    else  
    console.log(i+" is odd ");

 }


```

<br>

## Multiplication Tables

Write a for loop that will iterate from 0 to 10. For each iteration of the for loop, it will multiply the number by 9 and log the result (e.g. "2 * 9 = 18").

Bonus: Use a nested for loop to show the tables for every multiplier from 1 to 10 (100 results total).


```

for (let i=0 ; i< 10 ; i++)
{  
    console.log( i+" * 9 = " +i*9);
}; 
 // Bonus : 
 
for (let i=0 ; i<=10 ; i++)
{  
    for (let j=0 ; j<=10 ; j++)

    console.log( i+' * '+j+' = '+i*j);
   }; 


```

<br>

## The Grade Assigner

Check the results for every value from 60 to 100 - so your log should show "For 89, you got a B. For 90, you got an A.", etc.

``
const Result=["A", "B", "C", "D","F"];
let grade=[]; 
grade.push(95,40,58,70,100,65);
for ( let i=0 ; i<=grade.length-1 ; i++)
{
    if ( grade[i] >= 90 )
    console.log( "For "+ grade[i] + " you got a " + Result[0]);
    else if ( grade[i] >= 80)
    console.log( "For "+ grade[i] + " you got a " + Result[1]);
    else if ( grade[i] >= 70 )
    console.log( "For "+ grade[i] + " you got a " + Result[2]);
    else if ( grade[i] >= 60 )
    console.log( "For "+ grade[i] + " you got a " + Result[3]); 
    else 
    console.log( "For "+ grade[i] + " you got a " + Result[4]); 
};

```
