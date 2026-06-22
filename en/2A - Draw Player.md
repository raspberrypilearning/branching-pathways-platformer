## 2A - Draw Player

Draw your own costume for the existing **player** sprite in the starter project.

The **player** sprite already has code that handles gravity, jumping, and falling. Change the costume in these steps, but do not delete or change the code unless a later step tells you to, or the game might stop working properly.

## Step 1

> [!TASK]
>
> Open the [Starter project](https://scratch.mit.edu/projects/1331945689/editor/){:target="_blank"}.

## Step 2

> [!TASK]
>
> Select the **player** sprite in the sprite pane.
>
> ![Scratch Cat sprite selected in the sprite pain](images/player_sprite.png)
>

## Step 3

> [!TASK]
>
> Open the **Costumes** tab.
>
> ![The Costumes tab in Scratch.](images/tab_costumes.png)


## Step 4

> [!TASK]
>
> Open the costume menu and select **Paint** to add a new costume to the **player** sprite.
>
> ![The Paint option in the costume menu.](images/costume_paint.png)

## Step 5

> [!TASK]
>
> Draw a character for your platformer. Your player could be a person, robot, creature, animal, or simple shape.
>
> Use a clear outline and colours that stand out from your backdrop. Keep the design easy to recognise when it is small on the Stage.

## Step 6

> [!TASK]
>
> Delete the **Cat-a** and **Cat-b** costumes.
>
> ![Two Scratch cat costumes in costumes pane](images/cat_costumes.png)
>

## Step 7

> [!TASK]
>
> Check that your costume is facing sideways or is easy to turn sideways later. A platformer player usually moves left and right, so a side-on character will be easier to animate.

## Step 8

> [!TASK]
>
> On the **Code** tab, add blocks to set the starting position of your player. You can change this later
> ```blocks3
> when flag clicked
> go to x: (-200) y: (-120)
> point in direction (90)
> ```
>
> The `point in direction (90)`{:class="block3motion"} block makes the **player** face right. If your **player** starts on the right side of the screen, change the direction to `-90` so it faces left.
>
> > [!TIP]
> >
> > Start the **player** a small way above the floor so it drops down and lands on top. Do not place it directly on the floor: if it spawns too low and overlaps the floor sprite, even slightly, the **player** gets stuck inside it and the game breaks.

## Test

> [!TASK]
>
> Check that the **player** sprite shows your new costume on the Stage. If it is too large, change the **Size** number in the sprite pane to make it smaller.
