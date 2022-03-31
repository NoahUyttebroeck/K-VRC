# K-VRC
With this project you can syncronize a text with a spoken audio file and moving character.
This project is made to repicate K-VRC from [Love Death & Robots](https://nl.wikipedia.org/wiki/Love,_Death_%26_Robots) as an application.
And later used for a reallife robot counterpart. You can use this project not only for this purpose but you can also use it to create your own speaking character.
# Interface
![interface overview](https://i.ibb.co/dPGksqB/K-VRC-Interface.jpg)<br>
The interface exists of 3 main parts:
- [Display](#Display)
- [TextArea](#TextArea)
- [SettingsPanels](#SettingsPanels)
## Display
This is were your character is displayed. You can edit it's alignment with the yoffset constant or even write your own algnmentcode in: Window1->Controls->Canvas1->Paint
## TextArea
In here you can either choose a text file to use as read text or you can write it yourself and if you would like you could save your written text to your computer via the [SettingsPanels](##SettingsPanels)
## SettingsPanels
You can find these panels at the top- and bottom of the interface.
# Behavior
There are 9 default behaviors:
- Normal
- Happy
- Suprised
- Cheerful
- Suspicious
- Annoyed
- Embaresed
- WTF
- Ooh
## Add behavior
You can add your own behaviors by going inside your xojo project in App->Methods->LoadBehaviors and add the following code at the bottom of the file:
```BASIC
Behaviors.Add(new RobotBehavior([behaviorname], new Eyes([CLOSED eyesimage], [OPEN eyesimage]), new Mouth([CLOSED mouthimage], [OPEN mouthimage], [SMALL mouthimage])))
```
After doing this you can restart your application and your new behavior should be inside the behaviorlist
# Sound
Sounds are used to move a reallife character by outputting this analog signal in the right channel and other sounds like speech is outputted in the left channel.
# Add sound
You can also add your own sounds like you can with [behaviors](#behavior).
To add your own sound you need to make sure that there is only sound comming out of the right channel.
Put your sound file in the project folder under resources->snd
After doing this you can restart your application and your new sound should be inside the soundlist 
