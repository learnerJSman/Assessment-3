# Assessment-3
research repository

#Fun with classes

#CREATING ATTRIBUTES
#example class
Class Car:
   #attributes can be written just below the class header which will include it in every one created and will have the same instance value
   brand = 'volkswagon' #attribute1
   
   #self is an important key word as it makes the code refer to the instance instead of the class name
   #e.g. if i save model as being polo and saved under variable a. I can call a.model (being the instance if self is decleared), otherwise i cannot access it
   
   def __init__(self, model, price):
       self.model = model #attribute2
       self.price = price #attribute3
   
   #creating this car class will make 3 instances instead of 2 because of the extra attribute written under the class header

#example code    
a = Car(polo, 25,000)   
#this will have all the model, price, and brand instances

-----------------------------------------------------------------------------------------------------------------------------------------------------------------

#shorthand looping and forming a list from 
L = [mapping-expression for element in source-list if filter-expression] #found this template for list expression online
#the code above is the exact same as the one below
result = []
for element in source-list:
     if filter-expression:
        result.append(mapping-expression)
#example of this code  

example_list = [1,2,3,4,5,6,7,8,9,10]
result = []
for i in example_list:
    if i%2 == 0:
       result.append(i)
#As a list expression
result = [i for i in example_list if i%2 == 0]

#this code is a lot shorter and saves a lot of space. i have also seen that it runs faster than the above code, however, i do not know if this is true. I do want to learn more about this as well, especially how it works with classes

#researched what other shorthand expressions there where for more common things. found the IF else statement shorthand
if-expression if (condition) else else-expression 
#taking example from my assessment 2 code
   if close_ticket == 'yes':
        t_dict['Ticket Status:'] = 'closed'
   else:
        print('This ticket still needs to be resolved')
#short form way
[t_dict['Ticket_Status:'] = 'closed' if closed_ticket == 'yes' else print('This ticket still needs to be resolved')] 

#in this example the 1 line code looks more complex and would probably be easier to read. however, in most cases it would be much easier to read

--------------------------------------------------------------------------------------------------------------------------------------------------------------------

#Recursives in pynthon - where you calculate the same thing over and over
#using an import cache from the functools you can put it into memory, i found this to be a very interesting comcept

@cache #can used stored data in the cache instead of calulating everything again, first time seeing it was in the fibonacci resursive method but did not understand it till now

--------------------------------------------------------------------------------------------------------------------------------------------------------------------

#maps vs loops
#maps appear to be much faster as processing code so can be a lot better when you want to run a piece of code for everything you want to iterate over from my research, however, it only runs a function over something that is iterable
#example below

list = [1,2,3,4,5,6]

def function(a):
   add_one = a + 1
   print(add_one)
   
#using a for loop
for elements in list:
   add_one = elements + 1
   print(add_one)
   
#using map
map(function, list) #saying to run this function over every element in the list

#depending on use case a map may be better than a loop, however i see maps as being handy especially when you want to run the same function over 10 or 100's of list

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
#format function in pynthon

#in my assignment i used the what i called the 'f statement' where i can make a viarable (which can be changed) apart of my string
#my code in assigment 2

print(f"Your ticket number is: {i}")

#however it can also be written as

print("Your ticket number is: {}".format(i))

#i believe it is good to know both ways as i may see both in the future

----------------------------------------------------------------------------------------------------------------------------------------------------------------------
#so mqny different ways to do the same thing
#i researched some of the different ways to do the same thing. e.g. i want to copy a list contents and make a new list
my_new_list = my_list # this will not work as it as it doesn't copy the list it directs the new variable (my_new_list) to the same location as variable my_list

#things that do work
my_new_list = my_list.copy() #built in function that copies a list
my_new_list = my_list[;] #slices from index 0 to index (length-1) of the previous list
my_new_list = list(my_list) #constructs a list with the iterables in something that can be iterated over, in the case the old list

#this isn't just confined to list, i am not sure which is the best methods this early on however, learning about all the different ways of doing the same thing is very valuable






