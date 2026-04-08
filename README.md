# EcemNurBurguRollABallGame

Midterm Project

About the Project

In this project, I created a simple roll a ball game in Unity.

---

1) Setting Up the Scene

At the beginning, I created a plane as the ground and a sphere as the player.
I also added a Rigidbody to the player.


---

2) Moving the Player

I created a script called PlayerController.

While writing this code, I learned how to take input from the player.
At first I didn’t understand why we use FixedUpdate, but then I learned that physics must be handled there.

When I used:

`rb.AddForce(movement * speed);`

I saw that the ball finally started moving.

---

3) Camera Follow

After that, I added camera movement.

I wrote a CameraController script and used offset.
At first the camera was not following correctly, then I understood the importance of LateUpdate.

This part helped me understand how camera systems work in games becuse ı dont know before how to use camere in the player object.

---

4) Play Area (Walls)

Then I created walls using cubes.

Instead of creating each wall again, I duplicated them.

After I created small cubes as PickUp objects.

Then I added a rotation script.
When I saw them rotating, the game looked more alive.

I also created a prefab.
Before this, I didn’t know why prefabs are important, but now I understand they save a lot of time.

---

5) Collision System

Then I added collision detection.

At first, nothing worked.

Then I realized:

* I forgot to enable "Is Trigger"
* I didn’t set the tag correctly

After fixing these,

---

6) Score System (UI)

After that, I added UI text.

I created a count system and updated the text.
At first I got a NullReferenceException error.

Then I understood that I must connect the UI object in Inspector.

When I fixed it, the score started updating correctly.
This part helped me understand how UI works in Unity.

---

7) Enemy AI (NavMesh)

This was the most interesting part.

I created an enemy and added NavMesh.

At first I didn’t understand why the enemy was not moving.
Then I realized I forgot to assign the player.

After fixing that, the enemy started following me and it felt like a real game.

I also added:

* obstacles
* dynamic boxes

This helped me understand pathfinding and AI behavior.

---

8) Lose Condition

I added a system where if the enemy touches the player, the player loses.

When I first tested it, it didn’t work because I forgot the tag.

After fixing it, the game finally had a challenge.

---

9) Win Condition

I added a condition:
When all objects are collected → player wins.

Also, I removed the enemy after winning.

---

10) Problems I Faced

* NullReferenceException → fixed by connecting UI
* Player not moving → forgot Rigidbody
* Collision not working → forgot Is Trigger
* Enemy not moving → forgot to assign player

---

Extra

As an extra, I exported the mushroom and ghost objects I designed in Blender as assets into Unity, and I wanted to spruce them up a bit with a Mario-style concept.

---

Github

https://github.com/ecemnrbrg

