<img src="https://user-images.githubusercontent.com/84031027/235169420-40efb062-281d-47a5-b4c5-0e07b14aab5b.png" width="250" height="250">


## The Problem:

How many times did you buy a clothing item online, got really excited and then got super disappointed when it arrived, and it didn't fit as well as you imagined?

Unfortunately - While buying clothes online, it is difficult for a customer to select a desirable outfit in the first attempt because they can’t try on clothes before they are delivered physically.


## The Solution:

E-commerce websites can be equipped with virtual dressing rooms that allow users to try on multiple clothes virtually and select the best-looking outfit.

It's never been easier to look fabulous!!!


## The Approach:

I created a Virtual clothing assistant using Deep learning algorithms in order to help the costumers.

The user can select the clothing item he/she wants to wear and then upload his/her image of any pose they want, and the assistant will help to dress that human with his/her selected clothing item.


*So how exactly does it work?*
1.  	Input - We allow the user to upload his/her image and their clothing item’s image. 

<img src="https://github.com/shirsneh/virtual_clothes_try_on_assistant/assets/84031027/b2e797ff-805d-4fd0-a433-b09d9a23c2ce" width="600" height="250">

2.  	Cloth mask - We create a cloth mask with U2Net. 

<img src="https://user-images.githubusercontent.com/84031027/235325761-4e6dfaa7-6e75-4e2a-956a-55f27ab06d95.png" width="500" height="200">


3.  	Body position - We get a body position estimation and key points with OpenPose.

<img src="https://user-images.githubusercontent.com/84031027/235325802-be6a51e9-ba36-4dc9-be24-8ad26410d4f1.png" width="500" height="200">

</p>

4.  	Body segmentation - We segment the user body with U2Net.

<img src="https://user-images.githubusercontent.com/84031027/235325828-228be887-f96d-4d64-97f1-27db43ba1156.png" width="500" height="200">


5.  	Generating the result - ALIASGenerator uses these to create the requested image.

<img src="https://user-images.githubusercontent.com/84031027/235325853-24748a7d-3db6-47f8-8aa0-7ed0ba804328.png" width="500" height="200">

6.    Output - a new image of the user wearing the requested 
item.

<img src="https://user-images.githubusercontent.com/84031027/235325952-43226aa0-21bf-4a6c-b73d-8d0d643e5bd2.png" width="150" height="150">


## Project presentation

[project presentation.pptx](https://github.com/shirsneh/virtual_clothes_try_on_assistant/files/11360128/project.presentation.pptx)


## Resources

VITON-HD Dataset - https://paperswithcode.com/dataset/viton-hd


