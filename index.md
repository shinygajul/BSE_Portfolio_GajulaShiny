Raspberry Pi Object Detection
Software Program that helps find missing people using facial recognition. Utilizes Raspberry Pi and camera to detect target face using live camera feed and compares it with database. If target face detected, notification alerts user. 

| **Engineer** | **School** | **Area of Interest** | **Grade** |
|:--:|:--:|:--:|:--:|
| Srisukanya Gajula | Dublin High School | Electrical Engineering and Computer Science | Senior

![Headstone Image](https://bluestampengineering.com/wp-content/uploads/2016/05/improve.jpg)
  



# First Milestone
  

The first week focused on installing VNC, Putty, Visual Studio Code, and Raspberry Pi Imager. After connecting Raspberry Pi to the computer using a micro HDMI wire, I started coding with it on VS Code using python. The first task was a python program for using the Raspberry Pi Camera on VS Code. It was run on VNC using ssh commands and this successfully displayed the camera screen. Next, we used tensor flow to detect objects in a passed image. It takes a bmp image as an input and uses an interpreter to output a list of objects it believes to be in the image along with the certainty of it being that object. 

<iframe width="502" height="282" src="https://www.youtube.com/embed/h1WzSu9p8jA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


# Second Milestone

I brainstormed possible modifications that could be made to the project and settled on a Missing Person project. A program would consistently monitor the Raspberry Pi Camera feed to identify a target and output an image with a rectangle around the target's face. Dlib and OpenCV were implemented for facial recognition purposes, as the dlib is responsible for mapping out the coordinates of facial points and the OpenCV draws the rectangles around the faces that match the target face. The target face is saved in a folder and when "Enter" is pressed, the program takes a picture and identifies the faces in it and compares it with the target. 

<iframe width="560" height="315" src="https://www.youtube.com/embed/F4LTIHj898g" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


# Third Milestone

I focused on shifting the program from requiring a manual trigger to running on its own, devoid of human interaction. PReviously, the program would be triggered when the user pressed the "Enter" key. To mimic a "live feed", this trigger was replaced with a delay of 2 seconds. The program takes an image and retakes it shortly after comparing the faces in the previous image with the target face.

<iframe width="560" height="315" src="https://www.youtube.com/embed/V2SAfn3KXy4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
