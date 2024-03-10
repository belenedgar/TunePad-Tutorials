---
layout: layouts/activity.njk
tags: tutorials
category: Tutorial
title: "Under the Sea - Little Mermaid"
description: Learn about arpeggios in music and loops in Python by recreating the Stranger Things theme in TunePad
level: Beginner
time: 15-20 minutes
license: by-nc-sa
splash: /images/splash/stranger-things-splash.jpg
video: https://drive.google.com/file/d/1Er4rBmwG3Jj7FyCdDEIc8GfMkdx-Nuav/view?usp=sharing
slides: https://docs.google.com/document/d/1GJFpag52fC_8d6yRB6AliR6dF6JXxbo4yqCQENfbcxI/edit?usp=sharing
project: https://tunepad.com/project/27933
audio: https://api.tunepad.com/api/projects/27933/audio/
disclaimer: For educational purposes only. Based on Stranger Things Volume 1 by Kyle Dixon and Michael Stein (2016), Lakeshore and Invada Records.
---

# Step 1: Set up new Project
Open this [TunePad Project](https://tunepad.com/project/76846) and remix it so you are able to edit the project (make sure you are signed in to TunePad)

# Step 2: Drum 1
- Add a **Drum** cell to the project
- Select the **909 Drumkit**
- Create a rest that is 7 beats long
- Add 2 eighth notes playing the *ride* cymbal from the **909 Drumkit**
    - Find which number plays *ride*
    - Hint: An eighth note is half of 1 beat so... beats = 0.5
- Put the lines of code you've written in a for-loop as shown below:
```python
for i in range(6):
    # put the lines of code you've written here
    # make sure it's indented
```

# Step 3: Drum 2
- Add a **Drum** cell to the project, select **Percussion Sounds**
- This section is trying to add more dimension to the song by creating a fun and lively beat to play in the background
- Copy the code below into the cell
```python
for i in range(10):
    playNote(2, beats = 0.50)
    rest(1.00)
    playNote(2, beats = 0.50)
    rest(1.00)
    playNote(2, beats = 0.50)
    rest(1.5)
    playNote(2, beats = 0.5)
    rest(0.5)
    playNote(2, beats = 0.5)
    rest(0.5)
    playNote(2, beats = 0.25)
    rest(.75)
```

# Step 3: Frogs
- Add a **Drum** cell to the project, select the **Whistles** instrument
- Add a rest that is 1 beat
- Add 2 eighth notes playing the *frogs* sound from **Whistles**
    - Find which number plays *frogs*
- Add a rest that is 1 beat
- Add 2 sixteenth notes playing the *frogs* sound from **Whistles**
    - Hint: A sixteenth note is a quarter of 1 beat so... beats = 0.25
- Add a rest with 4.5 beats
- Put the lines of code you've written in a for-loop as shown below:
```python
for i in range(19):
    # put the lines of code you've written here
    # make sure it's indented
```

# Step 4: Bubbles
- Locate the **Bubbles** cell that was provided in the project. Inside you will see a for-loop holding a playSound() function that plays the bubble sound. Everything you write for this step will be inside the for-loop, meaning everything should be indented.
```python
playSound(3538, beats = 0)
```
- Copy the playSound function, and create two lines where beats = 0.25
- Add a rest with beats = 0.25
- Copy the playSound function, and create two lines where beats = 0.5
- Add a rest with beats = 0.5
- Copy the playSound function line, and create one line where beats = 1
- Add a rest with beats = 4.75
- Delete the original playSound() line that was given

# Step 5: Creating the Intro
- In this section you are going to write the introduction to the song!
- Add a **Keys** cell and select the **Marimba** instrument
- The code below includes the notes for the intro, copy the code into the cell you just created. Notice the beats for each playNote() are zero and will need to be changed!
```python
playNote(50, 0)
playNote(53, 0)
playNote(58, 0)
playNote([58, 50], 0)
playNote([58, 50], 0)
playNote(53, 0)
playNote([57, 60], 0)
playNote([63, 60], 0)
playNote([62, 58], 0)
playNote([53, 58], 0)

playNote(46, 0)
playNote(50, 0)
playNote(53, 0)
playNote([53, 58], 0)
playNote([53, 58], 0)
playNote(48, 0)
playNote([53, 57], 0)
playNote([51, 60], 0)
playNote([50, 58], 0)
rest(1)
```
- The introduction is an 8-beat rhythm, that’s played two times. Below is the sheet music that holds the rhythm for the introduction. We have added the number of beats that each note corresponds to in TunePad. Your job is edit each playNote() line to have the correct number of beats, based on the rhythm in the picture. *Remember that the pattern repeats, so after the first 8 notes, you will need to start the pattern again*
![pattern](https://github.com/belenedgar/TunePad-Tutorials/blob/3e6cd164a48a33086ea5329a74cb660dfb9bed4b/Pattern_A.png)
Goal: Understand how to create specific rhythm patterns in TunePad

# Special Challenge: Melody
Now we're going to add the melody
- Add a cell and select the **Brass** instrument (Synth -> Samples -> Brass)
- Click on the three dots in the right corner of your cell and click on **Toggle Note Names**. This will let you see the note names on the keyboard
- The code below includes the rhythm for the melody, which you should copy into the cell. Notice that each playNote currently has a 0 for the pitch, this will need to be changed.
```python
rest(16)

for i in range(2): #32
    rest(1)
    playNote(0, .5)
    playNote(0, 1)
    playNote(0, 1)
    playNote(0, .5)
    playNote(0, 1)
    playNote(0, 1)
    playNote(0, 1)
    playNote(0, 1)

    rest(1)
    playNote(0, .5)
    playNote(0, 1)
    playNote(0, 1)
    playNote(0, .5)
    playNote(0, 1)
    playNote(0, 1)
    playNote(0, 1)
    rest(1)

for i in range(2): #32
    rest(1)
    playNote(0, .5)
    playNote(0, 1)
    playNote(0, 1)
    playNote(0, .5)
    playNote(0, 1)
    playNote(0, 1)
    playNote(0, 1)
    playNote(0, 1)

    rest(1)
    playNote(0, .5)
    playNote(0, 1)
    playNote(0, 1)
    playNote(0, .5)
    playNote(0, 1)
    playNote(0, 1)
    playNote(0, 1)
    rest(1)

rest(1.5)
playNote(0, 1)
playNote(0, .5)
playNote(0, 1)
playNote(0, 1)
rest(3)

rest(1.5)
playNote(0, 1)
playNote(0, .5)
playNote(0, 1)
playNote(0, 1)
rest(3)

rest(1.5)
playNote(0, 1)
playNote(0, .5)
playNote(0, 1)
playNote(0, .5)
playNote(0, 1)

playNote(0, 1)
playNote(0, .5)
playNote(0, 1)
playNote(0, .5)
playNote(0, 1)

playNote(0, 1)
playNote(0, .5)
playNote(0, 1)
playNote(0, 4)

rest(1.5)
playNote(0, 1)
playNote(0, 1)
playNote(0, .5)

playNote(0, 1)
playNote(0, .5)
playNote(0, 1)
playNote(0, .5)
playNote(0, 1)

rest(1.5)
playNote(0, 1)
playNote(0, 1)
playNote(0, .5)

playNote(0, 1)
playNote(0, .5)
playNote(0, 1)
playNote(0, .5)
playNote(0, 1)

rest(1.5)
playNote(0, 1)
playNote(0, .5)
playNote(0, 1)

playNote(0, .5)
playNote(0, 1)
playNote(0, 1)
playNote(0, .5)
playNote(0, 1)

playNote(0, .5)
playNote(0, 1)
playNote(0, 1)
playNote(0, .5)
playNote(0, 1)

playNote(0, 1)

rest(15)
```
- The picture below is the sheet music for the melody with the name of each note written above it. Your task will be to find what number matches the note name and change the line in TunePad that plays that note with the correct number.
![melody](https://github.com/belenedgar/TunePad-Tutorials/blob/69c3a96a1767deaab0c2b214e0bbccad77363d82/Melody.png)

# Bonus Step 
- There's one last bonus step if you decided to complete the Melody!
- Once you've finished creating each cell, you need to switch to the **Tracks** tab at the top of your project
- Click the three dots on your intro track, and then click **duplicate**
![melody](https://github.com/belenedgar/TunePad-Tutorials/blob/1e739529b2a39961ecc4501680c76155cd82bafb/Bonus_Step.png)
- At this point you will have two copies of the intro track, leave one at the beginning and drag the other track over so it begins at measure 36, it will say *start: 140 beats*

# Try It
Open this project in TunePad <a href="{{project}}" target="_blank">{{ project }}</a>