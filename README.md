# Engineering_4_Notebook
## Vann's Engineering 4 Stuff! :)
## Getting the Pi Online
I had to use a hotspot, set yours to 2.5 GHz under AP Band if, on android, this took me a while to figure out the hard way.
## Dice Roller
This assignment was a basic one I got the logic to work. I used a simple random function and an if statement to kill the program. I would recommend using an online compiler to write the code as it takes lots of time to do it on the pi. Once I wrote it all I just copied it over. I've been doing lots of Java is CSA so the switch to Python was nice, it's all much easier in my opinion, or at least simpler. 
## Calculator
### Description
In this assignment, we used functions to do an array of operations on two use inputted numbers. I'd never used functions in Python before so this was a fun challenge. 
### Code
I'm going to talk about the two sections that gave me the most trouble. The first is taking the input from a function. 
`calculator.py`
```python 
print("Sum:\t\t" , doMath(a,b,1))
```
There a few parts to this. First, the print, we are really just telling python to print "Sum" and the return from doMath. The second big part is giving doMath its arguments, in this case, that is `a,b,1` a, and b are variable that are given their value by a user input earlier in the code. 1 is telling doMath what operation to do.  

Next is how I chose what operation to do.

`strings_and_loops.py`

```python
  words = input("Enter the sentence: ").split(' ')   #takes the input from the user and puts it in a list with a space in between
  for x in range(0, len(words)):  #a loop that runs for the length of the string
    for y in range(0,len(words[x])):  #loop that runs for the length 
        print(words[x][y])  #prints a letter from a part of the loop
    print("-")  #prints - in between words

 ```
C is the argument from the earlier print, it has a value of 1-5 at all times. Because of this we can use this simple solution, every value of c has an if/if else statment. The program finds the correct operation, completes it, and then returns it to be printed. 
### Lessons(s) Learned

- You can give a function values to work with (called an "argument"). You use `return` to spit back out the answer or whatever, not a `print`.
- Taking inputs is as easy as `x = input("Message")
- Rounding is very easy, just use `round(x,y)`, x being the number and y being the places to round to. 
## Quadratic Solver
### Description
In this assignment, we used functions with an array as the argument to solve a quadratic, or if no real roots exist, inform the user. 
### Code
`quadratic_solver`
```python 
if (discriminant < 0):   #if the discriminant is <0 it returns no roots
      return("There are no real roots")
    else:   #if there are real roots
        roots[0] = math.sqrt(discriminant)    #solving the quadratic formula
        roots[0] = (-1*num[1]) - roots[0]     #first root 
        roots[0] = roots[0] / (2*num[0])  
        roots[0] = round(roots[0],2)
        roots[1] = math.sqrt(discriminant)  #second root
        roots[1] = (-1*num[1]) + roots[1]
        roots[1] = roots[1] / (2*num[0])  
        roots[1] = round(roots[1],2)
        return(roots)       #returns the roots as an array
```

This is where the (inefficient) magic happens. Outside of this all that happens is taking user-input and printing the result of this section. What I'm doing is just solving the quadratic formula while giving its value to one of the two roots. After getting both roots it rounds them and then returns the array to be printed. 

### Lessons(s) Learned

- Arrays can be useful when dealing with lots of similar variables, the individual elements are easy to manipulate and they keep code simple. 
- One main mistake I made was making the framework and then building the solver, had I done it the other way around my code would have been simpler and more efficient. 
- You can return an array and then print it along with other things just like a normal variable.  
## Strings and Loops
### Description
In this assignment, we aked the user for a phrase and then we spit it apart letter by letter and printed it out with a hypen between the words.  
### Code
`quadratic_solver`
```python 
if (discriminant < 0):   #if the discriminant is <0 it returns no roots
      return("There are no real roots")
    else:   #if there are real roots
        roots[0] = math.sqrt(discriminant)    #solving the quadratic formula
        roots[0] = (-1*num[1]) - roots[0]     #first root 
        roots[0] = roots[0] / (2*num[0])  
        roots[0] = round(roots[0],2)
        roots[1] = math.sqrt(discriminant)  #second root
        roots[1] = (-1*num[1]) + roots[1]
        roots[1] = roots[1] / (2*num[0])  
        roots[1] = round(roots[1],2)
        return(roots)       #returns the roots as an array
```

This is where the (inefficient) magic happens. Outside of this all that happens is taking user-input and printing the result of this section. What I'm doing is just solving the quadratic formula while giving its value to one of the two roots. After getting both roots it rounds them and then returns the array to be printed. 

### Lessons(s) Learned

- Arrays can be useful when dealing with lots of similar variables, the individual elements are easy to manipulate and they keep code simple. 
- One main mistake I made was making the framework and then building the solver, had I done it the other way around my code would have been simpler and more efficient. 
- You can return an array and then print it along with other things just like a normal variable.  



