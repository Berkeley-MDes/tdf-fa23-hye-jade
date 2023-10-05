# [Week of 10/05/2023] Proton2 #3
🪷TDF Mindful Meditation Bloom 
Project Overview
Meditation Bloom aims to amalgamate technology, aesthetic, and mindfulness, crafting a transformative physical and mental experience. It is a meditation-assistive device that provides a multi-sensory experience by integrating visual, tactile, and audial cues, thus enhancing the user's focus and immersion during the meditation process.


Components:
1. Meditation Flower:
Function: 
Opens and closes in synchronization with the prescribed meditation breathing pattern.

Design: 
Resembling a delicate flower that blooms and retreats, providing a visually calming and metaphorically rich imagery.

Technology:
Utilizes mechanical petals that are controlled by a microcontroller, ensuring smooth and synchronized movement.

Lighting:
Subtle and adjustable lighting that complements meditation moods and provides ambience.

2. Wristband
Function: 
Vibrates subtly, aligning with the meditation breathing pace and providing tactile feedback for breathing synchronization.

Design: 
Ergonomic, lightweight, and non-intrusive, ensuring comfort and aesthetic appeal.

Technology:
Employs a precision haptic motor which can adjust vibration intensity and pattern, to avoid startling the user and to align accurately with the meditation rhythm.
Target Audience
Primary:
Individuals seeking innovative and immersive meditation experiences.

Secondary:
Wellness centers, therapists, and yoga studios that could utilize the device to enhance their service offering.
User Interaction
The user initiates a meditation session via a mobile application, selecting or customizing their breathing pattern and pace.
The Meditation Flower responds by opening and closing in tandem with the selected breathing pattern, while simultaneously illuminating to establish a serene environment.
The wristband vibrates in sync with the pattern, providing tactile cues to assist the user in maintaining the prescribed breathing rhythm.

Objectives
Enhance the user’s meditation experience through multi-sensory engagement.
Provide a visually pleasing apparatus that doubles as a decorative piece when not in use.
Facilitate consistent and focused meditation through synchronized cues.

Key Features
Breathing Flower:
The Meditation Flower is able to close and open up based on selected meditation patterns with a built-in lighting that is capable of changing colors according to the user’s selection.

Vibrating Wristband:
The wristband vibrates subtly on the user’s wristband according to the selected meditation patterns.

Synchronization:
Ensures that visual and tactile cues are precisely synchronized with the selected meditation pattern.

User Customization:
Allows the user to select and customize breathing patterns, vibration intensity, and light intensity.

App Integration: 
(Might now able to realize in this round of iteration, but is open up to further development)
Enables the user to control, customize, and track their meditation sessions via a dedicated app.

Design Specification
Technological Challenges:
A smooth mechanism for the Meditation Bloom to open and close up.
Robust and quiet motor for the Meditation Bloom to ensure non-disruptive drive of the mechanical part.
A reliable communication protocol between the Meditation Flower, wristband, and app, ensuring synchronized operation.
High-precision haptic technology in the wristband for subtle and accurate vibrations.
Energy-efficient LED technology for the Meditation Flower, ensuring sustainable operation and longevity.

Mechanical Flower
Brainstorming of forms
2D Flower


3D Flower

Geek's Valentine's day: Everblooming Mechanical Flower Garden

Ball-shaped flower
Something similar to the Hoberman sphere:
https://www.youtube.com/watch?v=-DsHk_iR_xU

Pendant flower (Like a pendant light)


Circuits & Code


In terms of the coding, we plan to rely on the rotating servo motor to control the mechanical parts to mimic the flower opening and closing.

Wristband

🦾Mechanical
A simple wristband can be done through laser cutting plywood and bend it in shape:


Circuits & Code
For the wristband, it has a vibrator motor built inside for vibration guiding on the wrist. The vibration pace will be in sync with the motion of the flower, working as a secondary guide device for meditation.

The circuit (and code) of the wristband is quite straightforward: by connecting vibrator motor to photon 2 and set the pace to link to the meditation pace. For the code, we can build a front-end web page that has several buttons on it. By controlling the buttons users will be able to test, begin or end the vibration.


We did a little test of the vibrator motor and it worked like this:





# [Week of 09/28/2023] Proton2 #2

This week, we gained insight into using Proton2 by making an LED work. Additionally, we conducted a brainstorming session for ideas for our team project 2. It was a very smooth and enjoyable environment for brainstorming because there weren't many constraints other than time limits, and all our group mates were very open and supportive of the ideas we brought to the table. After gathering all the ideas, I had a hard time selecting only three of them because every idea sounded exciting. It was a pleasure to see all these interesting ideas, making me look forward to our next project!

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/0bb3c259-96d4-46ad-9857-b2f92f970533)


Also, we had a chance to listen Adrian Freed's(http://www.adrianfreed.com/, Research Director of UC Berkeley's Center for New Music and Audio Technologies) lecture. He showed many examples of electrical textiles could be used in wearable devices. It was so interesting!

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/e4c1ff83-310c-4d81-b24f-0c7ba1e64747)


![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/715694c6-35a6-459f-a162-0d099e3b0c8b)


![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/00c7a1a1-9c2f-435a-b532-bb3b2334a52a)


![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/dd72db09-708f-4de2-94d4-2b90a3e6f2d9)


![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/aaf0e047-587d-428b-bfc8-0e7a44bcea14)



I assisted my classmates during the class based on my understanding of Arduino from my past experiences. I helped with tasks like uploading code to the microcontroller and understanding the polarity of the LED/.... I hope to have more opportunities to help my classmates as time goes on. During the brainstorming session, I contributed numerous interesting ideas. Additionally, I made sure to listen carefully to others' ideas and incorporate my own to make them clearer and more feasible.


# [Week of 09/21/2023] Proton2 #1

We'll start to play with proton! 

I tried to do the wifi connection at home, but Particle couldn't find the network. 

I tried to solve the problem but I couldn't at the end... 

I will organize the process anyway!


1. Update the particle device
![화면 캡처 2023-09-21 082532](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/75b90e94-4192-4017-b5d7-ab358434a15a)

2. Create my device
![화면 캡처 2023-09-21 082702](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/a86fcf5a-c245-4da1-a5d7-6a4c0fc7e36f)

3. Give a name! 
![화면 캡처 2023-09-21 082721](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/f70a8e3a-0c02-4251-b8fa-570cf5aa4f35)

4. Tried to get wifi at home but it didn't work.... and I tried from process1 but it showed like this
![화면 캡처 2023-09-21 091136](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/5f5a1fe2-56bf-4d1e-bca9-ba4fc3b349a8)


I need to take time work more on this. I think I should find another network from visiting my friends home.


# [Week of 09/14/2023] Computational Design #3

Video Submission day! 
I have every progress for this week in this video : 
https://youtu.be/qrvmXjAUm_U


# [Week of 09/07/2023] Computational Design #2
**Good things about Grasshopper**

Common 3D modeling programs, including Rhino, work in a clear-cut beginning-to-end fashion, like drawing guidelines, then points, then lines, and finally creating faces. Therefore, it is difficult to go back to that point in time and make corrections in the case of past work that has already passed to some extent(even if there are some differences between programs). Therefore, perfect design must precede 3D modeling, and inevitably, if the design is changed during 3D modeling, the work process that has been carried out so far must be discarded and returned to a point in time a long time ago.

This exposes the weaknesses of common 3D modeling programs in two respects. First, since all of the previous work is invalidated, the work time increases exponentially whenever the design is changed during the 3D modeling process. Second, although the design can be improved in the process of concretely expressing what was in the imagination or sketch through 3D modeling, creative thinking to seek a better design is completely abandoned during 3D modeling due to the above reasons.

However, in Grasshopper, **all individual tasks are done through components**, and the whole task is carried out in a way that connects the components together. It is exactly the same method as the algorithm learned in math class in school. Here, all the components from the first utilized component to the last component of the work remain connected to each other on the land called the canvas. Therefore, in Grasshopper, unlike the other programs described above, it is possible to modify the work at any point in the past at any time.

With this, Grasshopper perfectly overcomes the two weaknesses of common 3D modeling programs described above.

**First, during the process of 3D modeling, the design can be changed at any time by manipulating past components that have already passed, so even if the design is changed, the working time does not increase at all.** If you are only changing the numerical value of a component, it only takes 1-2 seconds. Even if the design is drastically changed, the work time is not increased due to things unrelated to the change work because only the parts that need modification can be cut and replaced with new components.

**Second, creative thoughts can be made at any time to improve the design while doing 3D modeling, and it can be easily reflected in the design since the work efficiency according to design change is very high.** In addition, even if only the numerical value of a specific component is changed in various ways, various variations with the same design identity can be created. Furthermore, it is possible to create a new design that simultaneously contains the identity of the two designs by well connecting the components that make up the two unrelated designs.

This week, I explored Grasshopper that I didn't really know how to use.

**Components**

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/426d6b0a-893c-4751-91ee-ac8d08e5ba4a)

When a component is selected by left-clicking, the component turns green and is activated in the Grasshopper.

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/abd3a606-2c6b-4e85-9a4c-04f67a6aa3ee)

You can know the current state through the component color.
- light gray: works fine
- Dark gray: Component preview OFF state
- Orange: Components with minor issues, issues need to be identified and resolved
- Red: A component with a big problem, it is highly likely that an incorrect value was entered.

**Wire**

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/006243be-99e9-4806-acfc-1a70ffcf1818)

The data structure can be inferred by looking at the shape of the wire.
- 1 item in 1 branch: single line
- 2 or more items in 1 branch: double line
- Two or more branches: dotted line

  ![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/bd731c37-5321-4061-b34e-be9c82cf7896)

To break a connected wire, hold down ctrl while dragging.

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/98f50127-3013-4b7a-8abc-2320b5e6ab4e)

If you want to connect two or more wires at one place, hold down the shift key while dragging.

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/0288f753-e9f9-4a40-9283-e3ea2fed5cc6)

If you want to move two or more wires to different places at once, drag them while pressing Ctrl+Shift at the same time.

**Set&Bake**

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/328f5654-f76a-4664-bb80-83167d7eaea8)

The meaning of Set is to bring information from Rhino to the Grass Hopper. To set, after creating the information to be set and appropriate components in Grasshopper, select the information to be set in Rhino, right-click and press the set button. Set One is used to enter one piece of information, and Set Multiple is used to enter multiple pieces of information.


![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/f5796cbb-6cc2-4136-9afa-704cf3cd976e)

Bake, on the other hand, is used when exporting from Grasshopper to Rhino. Before Bake, the form seen in the Rhino window is just a preview before it is implemented in Rhino, literally a preview, and information is actually output only when Bake is performed. For Bake, select the component to export, open the radial menu, and select the fried egg shape at the bottom right.

**Radial menu**
To open the radial menu, use Ctrl + Space bar or middle mouse wheel click.

- Disable/Enable Preview: Disable/enable preview, Ctrl+Q is convenient.
- Group: Grouping creates a background color, which is good for highlighting or distinguishing algorithms. If you right-click the background color part and enter text in the empty space at the top, you can also set the name you want. You can also -change several properties or change the background color.
- Cluster: A cluster is a function that organizes repeated parts or overly complicated algorithms to express algorithms more clearly.
- Preferences: The Grasshopper settings window appears.
- Navigate: similar to the game's minimap
- Disable/Enable: Disable/enable component
- Zoom: Similar to Rhino's zoom_selected function, fills the Rhino window with the part corresponding to the component selected in Grasshopper to find it.


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

