# [Week of 09/07/2023] Computational Design #2
**Good things about Grasshopper**
Common 3D modeling programs, including Rhino, work in a clear-cut beginning-to-end fashion, like drawing guidelines, then points, then lines, and finally creating faces. Therefore, it is difficult to go back to that point in time and make corrections in the case of past work that has already passed to some extent(even if there are some differences between programs). Therefore, perfect design must precede 3D modeling, and inevitably, if the design is changed during 3D modeling, the work process that has been carried out so far must be discarded and returned to a point in time a long time ago.

This exposes the weaknesses of common 3D modeling programs in two respects. First, since all of the previous work is invalidated, the work time increases exponentially whenever the design is changed during the 3D modeling process. Second, although the design can be improved in the process of concretely expressing what was in the imagination or sketch through 3D modeling, creative thinking to seek a better design is completely abandoned during 3D modeling due to the above reasons.

However, in Grasshopper, **all individual tasks are done through components**, and the whole task is carried out in a way that connects the components together. It is exactly the same method as the algorithm learned in math class in school. Here, all the components from the first utilized component to the last component of the work remain connected to each other on the land called the canvas. Therefore, in Grasshopper, unlike the other programs described above, it is possible to modify the work at any point in the past at any time.

With this, Grasshopper perfectly overcomes the two weaknesses of common 3D modeling programs described above.

First, during the process of 3D modeling, the design can be changed at any time by manipulating past components that have already passed, so even if the design is changed, the working time does not increase at all. If you are only changing the numerical value of a component, it only takes 1-2 seconds. Even if the design is drastically changed, the work time is not increased due to things unrelated to the change work because only the parts that need modification can be cut and replaced with new components.

Second, since the work efficiency according to design change is very high, creative thoughts can be made at any time to improve the design while doing 3D modeling, and it can be easily reflected in the design. In addition, even if only the numerical value of a specific component is changed in various ways, various variations with the same design identity can be created. Furthermore, it is possible to create a new design that simultaneously contains the identity of the two designs by well connecting the components that make up the two unrelated designs.



# [Week of 08/31/2023] Computational Design #1
I learned how to use Rhino, at first, it was also difficult to get a grip on the four quadrants on the Rhino's screen.

**WHY I can only see the circle in the middle?**

When I first opened Rhino, I was surprised as I saw only a simple circle drawn. 
With the help of design specialist, I typed 'grasshopper' in the command prompt to open the Grasshopper program. Upon pressing the green button, all the objects became visible. According to the design specialist, it's common to keep the green button off and choose to drag and view only the parts you need in Grasshopper.

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/6ae8f7de-611e-46e0-8bab-dccc261781ea)

The parts that appear as orange lines in Grasshopper don't have any effect on the code, design specialist said. So, it's good to group and disable them using Ctrl+G. By going through this disabling process, the program becomes lighter and rendering speeds up. In Cody's case, he had designed the train system for Anaheim. If he turned on all interactions at once in Grasshopper, it would cause a system crash.

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/174e1765-61c1-4ea1-b527-c9ea29bbb770)


As I explored the Grasshopper program, it's considered a tool for parametric modeling and relationship design. The aspect that stood out to me was the ability to visualize the code, allowing you to see the relationships between objects at a glance.


**Command function**
- Since there are too many icons and functions in the program, it's convenient to use "Command" function like this.
![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/6c751f0b-4a0e-49b3-88e4-ebc7091ff079)

I used more commands below.
- 4View (only for perspective view, 'wireframe' for others)
- _Group(or Ctrl+G)
- Grasshopper(to open Grasshopper)
- etc...

**Customizing Phonestand to my phone**
1) Measuring
I need to consider the phonecase sizes as well. It was --> H * W * T = 150 * 75 * 12

*"Well...While taking pictures of the process of measuring the phone size with an iPad, I felt once again that I needed a phonestand!"*

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/d4b9ce03-f009-4048-87c4-4015cc0f9ad1)
![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/bef15227-1e0d-497c-8bd4-d5670c5fbed3)
![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/2f1ece46-c557-4a4c-8807-284da8a936e8)

3) Adjusting Phone Size
![phone size](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/befff3fe-b485-431c-bf37-f68b12968135)

4) Adjusting Student Activity Range and Height 
![1100_1187](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/e7ee61c2-c485-4f4f-8a69-4f633b9790f1)
![height](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/e000db09-ff4a-4a5c-8126-063ec8fdb8c0)

**Bake**
- To make it as a 2D model and to select for export, I should 'bake' it in Grasshopper.

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/5bb61273-1bd1-4723-9375-ccb4f9ff0cfe)


**Placing objects**
- Set Layer and color code it. When you export, it will automatically be red and easy to adjust for cutting.

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/4180ee33-464c-40d4-bf11-ad06722d0b2c)

- The pieces were placed out of the board, so I used "move to 0" so that it is visible in the illustrator.
  
![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/f50213e8-9f14-40c6-9779-8feddc2b3f64)

- The grid didn't show up, so typed "Grid" and changed "ShowGridAxes=Yes", "ShowGrid=Yes"
- It's Cody's little tips! His favorite settings are like this, and it is convenient to use! 'Onsnap' makes it easier to draw lines.

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/8bbd3a19-0737-411e-930c-bd7ca3a847a7)

**Export**

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/e37fbe4f-fe9b-436f-a574-95a1455404cc)

**Illustrator**

- Document settings : 32 * 18 inches (our laser cutter's size)
  
![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/904ce791-5629-4537-a4de-2825781d86a3)

- Turn on the [View > CPU preview] to make missing lines visible


**Settings for Laser cutting**
- It is helpful to check which area is available to reuse material. (click "Focusview" and set where do you want to set the laser.)

  ![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/92ca893f-f58b-477f-a1a4-3e2ff6f01820)
![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/6cbd9f19-6633-41f3-b2b7-0f1313793466)

- I changed my design's location a little bit to adjust with the reuse material.

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/be58a5ce-9b4d-4222-a0a9-a77bb7a623da)

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/7f22c7a1-a01f-4e58-ae9f-c8b9363e0c0a)

- Material setting

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/11ea8a9a-26ff-4f4a-b741-347e85847e13)

- This is the setting for intensity. I could set like this, and it's better to check with fingers after cutting to see if it is well cut.

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/ff57d999-edf2-415a-9217-f4ebe34ad9ed)

- Line thickness should be 0.001pt, and Blue and Black line has different function. Blue will just follow lines and engrave it, black will engrave all along the lines and the surface inside.

**Preparation!**
- I turned on the laser exhaust switch, checked if air flows, and turned on the compressed air switch!
![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/08b02eee-531a-4817-88a0-61265b735bf8)

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/4938e296-7405-4050-ab9a-983de82ae628)

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/16fa1790-0aad-447b-8447-991e50d23c2d)

- I found this sign later, I was almost playing around but I realized that I shouldn't have done that.
![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/75b36ee4-c161-4b66-b7c5-b65273f3734b)


**Results**

Succeed! But I want it to be more study. I thought it would be better to adjust the hole size or add a few more slots to make it fit a bit more snugly. Also there were too much soot in the wood!!!

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/4cc3e614-81b7-45db-8c80-5c65e48772f8)
![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/b3659a51-d768-4d0c-9657-be46945dc458)
![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/feb05ed8-3685-40e6-9f1f-f1ec0b99df17)



**In this writing, reflect thoughtfully on your personal performance since last week. Did you take an opportunity to help out a classmate?  Were you able to meet your personal expectations?  What helped or hindered your performance?  Use full sentences.**

During my undergraduate years, I had the opportunity to briefly experience using laser cutting and Rhino. I thought it wouldn't be too difficult, but it turned out to be more challenging than I anticipated. (I faced difficulties from the moment I opened the Rhino program.) Rather than meeting my personal expectations, my proficiency with Rhino was still quite low, which was disappointing. However, I plan to look for tutorials and put in more effort to improve in the future.

What truly helped with my progress was the assistance of the design specialist. When I visited the makers space in a somewhat urgent situation, the design specialist patiently guided me in a way that was easy to understand, enabling me to complete the task. I regret not seeking help earlier and I've realized the importance of being more proactive in asking questions and seeking advice in the future.

One positive aspect I want to highlight about my achievements is that I diligently documented the usage and settings of Rhino, Grasshopper, and laser cutting techniques through photos and notes, so that I can remember them when using them in the future. Additionally, I find it enjoyable to explore GitHub, which I'm using for the first time. While I started the assignment a bit late and didn't have the chance to 'physically' assist my classmates, I was glad to help a few friends with things like finding information about laser cutting reservations or setting up GitHub repositories.

**In this writing, reflect thoughtfully on your cohort's performance since the week.  Was there anything that surprised you? Are you grateful for assistance from a classmate? Is there anything that you can contribute that would improve the experience? Use full sentences.**

 Actually when I first opened Rhino, I only saw a simple circle and couldn't see any objects. Like this, I found it difficult to follow the assignment instructions, as there were no specific solutions provided. Also, I had to search for information from various sources like the wiki, GitHub, bcourse, Google Drive, and more, which made the task challenging. I was impressed by how everyone seemed to easily find the necessary information and complete the assignment.
 
 It was also nice to see how people were reusing materials effectively even if no one told to do that. Furthermore, when I mentioned that I was having trouble finding time for laser cutting, a friend offered to split their reserved time with me. (In the end, I managed to make a reservation myself.) 
 
 It would be great if we have a clear outline of exactly what tasks need to be done by the deadline.(Maybe I could do that!) Also, I hope I can help friends around me and contribute to their learning after becoming more familiar with the software.

