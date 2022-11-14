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
   
   #creating this car class will make 3 instances instead of 2

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
result = []
for i in range(10):
    if i%2 == 0:
       result.append(i)
#As a list expression
[i for i in range(10) if i%2 == 0]

#researched what other shorthand expressions there where for more common things. found the IF else statement shorthand
if-expression if (condition) else else-expression 
#taking example from my assessment 2 code
   if close_ticket == 'yes':
        t_dict['Ticket Status:'] = 'closed'
   else:
        print('This ticket still needs to be resolved')
#short form way
[t_dict['Ticket_Status:'] = 'closed' if closed_ticket == 'yes' else print('This ticket still needs to be resolved')] 

--------------------------------------------------------------------------------------------------------------------------------------------------------------------

#Recursives in pynthon - where you calculate the same thing over and over
#using an import cache from the functools you can put it into memory

@cache <-- can used stored data in the cache instead of calulating everything again

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

#depending on use case a map may be better than a loop




