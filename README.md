# Drawer-WebApplication
Drawer-Web-Application
canvas drawing web-based application

*The steps required to run your code

-1.Install Vuetify
-2.Install Axios
-3.Run Back-end first so it runs on port 8080
-4.Then Run Front-end so it runs on port 8081
# Class Diagram
![image](https://user-images.githubusercontent.com/60818439/126724179-11708b6f-da37-4304-aee8-d2366218f8ce.png)

# how we have applied the required design pattern

1-We used Shape Factory design pattern: Service Class is the shape factory for shapes to generate shapes and to make any operation on shapes(delete, copy…).</br>
2-We used singleton design pattern: to do only one object of service class.
3-We wanted to use prototype design pattern on shapes to make copy of them.
But that causes a problem in frontend; it makes (flicker problem).
So, we made a copy of our shapes in the frontend to be more efficient for the user.
![image](https://user-images.githubusercontent.com/60818439/126724339-eaf05ce3-a2ad-4b1d-8ad2-514d9fc299a4.png)

## snapshots of UI
![image](https://user-images.githubusercontent.com/60818439/126724415-7b10bed9-5743-4105-9d9b-4ffe02b191b9.png)
## some guides 
1.you cannot draw unless you choose shape first</br>
2.you can do move , recolor, or copy or…</br>
not only one time on click like if u click delete you can delete shapes as much as you want but you cannot do anything -like drawing- except delete</br>
3.Recolor Program will take new colors from fill color and stroke color in left of canvas</br>
4.copy When you make copy, u have two options:</br>
*First, one-click on shape then new copy will be created in front of the old one </br>
*Second, user can click and drag which will make user move the new copy anywhere he want </br>
*Like shown below one-click on circle , click and drag on square </br>
![image](https://user-images.githubusercontent.com/60818439/126724439-e5686453-9f94-4a24-a921-486281780da1.png)

5.Move and Resize
Just click on shape and drag and it will happen
6.Save & load
There are two buttons to save one for XML and other for JSON And same for load

We save xml as file name “shapes.xml” and Json as file name “shapes.json”
These two files are created in backend folder.
Cause of time we cannot make user choose where to save or where to load from, but program still save and load correctly as XML and as JSON
U can test it by save drawing as json and another one as xml.

