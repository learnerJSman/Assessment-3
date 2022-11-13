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

import # can be used to not only import pynthon codes but can also be used to import your own pynthon variables


