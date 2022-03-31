# K-VRC
# Interface
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
```xojoscript
Behaviors.Add(new RobotBehavior([behaviorname], new Eyes([CLOSED eyesimage], [OPEN eyesimage]), new Mouth([CLOSED mouthimage], [OPEN mouthimage], [SMALL mouthimage])))
```
# Sound
# Add sound
