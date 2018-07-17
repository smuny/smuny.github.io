---
layout: post
title:      "Concepts in OOR"
date:       2018-07-17 20:21:45 +0000
permalink:  concepts_in_oor
---


I've been stuck on OO Properties, Meowing Cat Lab

class Cat
  attr_accessor :name
  
  def meow
    puts "meow!"
  end
  #def name=(cats_name)
  #@actual_cats_name = cats_name
  #end
  #def name
  #@actual_cats_name
  #end
end

maru = Cat.new
maru.name = "Maru"
maru.meow

What I was able to understand was the concept. Under a class, you are creating a list of things for that specific object. 
It has to be a general structure that when it is used outside of the class, it can be defined more specifically. One way it help me understand this was to change the name of the class to Human.

There is a class Human.
The attributes of a Human can be Name, Height, Sex, Nationality

so it can be written as 

class Human
 attr_accessor :name, :height, :sex, :nationality
 end
 
 Then outside of the you create different type of people
 
For example,

person1 = Human.new
person1.name = "Hannah"
person1.height = "165cm"
person1.sex = "female"
person1.nationality = "Chinese"

person2 = Human.new
person2.name = "Paul"
person2.height = "195 cm"
person2.sex = "male"
person2.nationality = "Korean"
