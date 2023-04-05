# Markdown-assignement
notes for the oop unit

#### OOP vs procedural programing
___
* OOP focuses on how to manipulate the data of the object rather than the logic required to manipulate them
it does this through the use of classes and objects

## Objects
___

__Object’s Data → called: attributes__


__Object’s Code → called: methods__
___
### The objects have attributes and methods 

eg creating a object for Dog

__attributes:__
Dog may have the following attributes
* Name
* Color
* Breed
* isHungry
* isThirsty

__methods__ 
Dog may have the following methods
* bark()
* eat()
* sleep()
___
## Classes
___

#### Creating a Method for a Class
```python
  class Person:
    def greet(self):
      print(‘Hello, how are you?’)
    #end of greet
    #end of class Person
    p = Person()
    p.greet() # outputs the greet message …

```

# Encapsulation
___
* Information Hiding: Restricting the access to the classes/objects’ certain attributes and methods.
*   Why?
Data Protection
Restricting certain methods to be callable
The way to encapulate somthing is by adding __ in front of it
___
# OVERRIDING
 ___
##### Overriding - two methods with the same method name and parameters (redefining)
eg
```python
class Bear:
		def sound(self):
			print(‘roarrrr’)
	class Dog:
		Def sound(self):
			print(‘bark’)
		
	Def makeSound(animal type):

```

___
## Polymorphism
___
#### Polymorphism: A method that can be used across different classes and objects that is dependent on parameters

__rep__() base function: 
overrides object and is used to make it printable  

###### IMPORTANT
* Anytime there is a __str__ used there should also be __repr__


## interable objects 
___
#### eg deck of cards

```python
class Deck:
	… Code …
	def __iter__(self):
		return self

	def __next__(self):
		self.__index += 1
		if self.__index == len(self.__cards):
			self.__index = -1 # index reset
			raise StopIteration
		else:	
			return self.__cards[self.__index]

```

##### __Inter()__  and __next()__ are used to iterate 

___



