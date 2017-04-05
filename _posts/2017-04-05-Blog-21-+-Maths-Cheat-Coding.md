---
title: Blog 21 + Maths Cheat Coding
layout: post
author: liam.potter
permalink: /blog-21-+-maths-cheat-coding/
source-id: 1NkUm15f7a2e_L1jm95cUdGrhpslUE7YwDrqPpoA8DCE
published: true
---
<table>
  <tr>
    <td>Title:</td>
    <td>Making a 'Maths Cheat'</td>
    <td>Date:</td>
    <td>30/3/17</td>
  </tr>
</table>


<table>
  <tr>
    <td>Starting point:</td>
    <td>No coding</td>
  </tr>
  <tr>
    <td>Target for this lesson?</td>
    <td>To know how to do the Maths Cheat so I can do it on a later date at home.</td>
  </tr>
  <tr>
    <td>Did I reach my target? 
(add details to "Lesson Review")</td>
    <td>Yes as I now know how to do the Maths cheat coding and think I can do it at home.</td>
  </tr>
</table>


<table>
  <tr>
    <td>Lesson Review</td>
  </tr>
  <tr>
    <td>How did I learn? What strategies were effective? </td>
  </tr>
  <tr>
    <td>I learnt with a simple strategy, in short, it was to firstly try what I think is right, then secondly look at why it is wrong and what I should change then I see what Mr Keen has done and change my work accordingly then I check through and see how it works and if it doesn't work I look at what the website wants me to fix.</td>
  </tr>
  <tr>
    <td>What limited my learning? Which habits do I need to work on? </td>
  </tr>
  <tr>
    <td>I think that my confusion in some coding parts held me back but thanks to the guidance that Mr Keen gave to us I was able to get through it.</td>
  </tr>
  <tr>
    <td>What will I change for next time? How will I improve my learning?</td>
  </tr>
  <tr>
    <td>Next time I will try and experiment more and tidy up my work so that it is more presentable.</td>
  </tr>
</table>


from math import pi

def main():

  greeting()

  while True:

	response = select_function()

	print(response)

 

def greeting():

  print("Hello. I am a homework cheat.\n How can I help you?")

 

def select_function():

  print("These are my functions:- ")

  print("1: rectangle_perimeter")

  print("2: rectangle_area")

  print("3: cubic_volume")

  print("4: circle_area")

  print("5: circle_circumference")

  print("6: triangle_area")

  result = input("Please select a number.")

  while True:

	if result == "1":

  	a= input("What is the height?")

  	b= input("What is the length?")

  	return (rectangle_perimeter(a,b))

	elif result == "2":

  	a= input("What is the height?")

  	b= input("What is the length?")

  	return (rectangle_area(a,b))

	elif result == "3":

  	h= input("What is the height?")

  	w= input("What is the length?")

  	d= input("What is the depth")

  	return (cubic_volume(h,w,d))

	elif result == "4":

  	a= input("What is the radius?")

  	return (circle_area(a))

	elif result == "5":

  	a= input("What is the radius?")

  	return (circle_circumference(a))

	elif result == "6":

  	a= input("What is the height?")

  	b= input("What is the length?")

  	return (triangle_area(a,b))

	else:

  	print("Please select more carefully.")

  	break

def rectangle_perimeter(l,w):

  return (l + l + w + w)

 

def rectangle_area(l,w):

  return ((l*w) + " units squared")

 

def cubic_volume(h,w,d):

  return ((h*w*d) + " units cubed")

 

def circle_area(r):

  return ((pi*(r*r)) + " units squared")

 

def circle_circumference(r):

  return (2*pi*r)

def triangle_area(a,b):

  return ((a*b/2) + " units squared")

 

main()

