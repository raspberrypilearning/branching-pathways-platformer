## 2B - Upload Player

Upload an image as a costume for the existing **player** sprite in the starter project.

The **player** sprite already has code that handles gravity, jumping, and falling. Change the costume in these steps, but do not delete or change the code unless a later step tells you to, or the game might stop working properly.


## Step 1

> [!TASK]
>
> Open the [Starter project](https://scratch.mit.edu/projects/1331945689/editor/){:target="_blank"}.

## Step 2

Make sure you already have an image you want to use saved onto your computer.

> [!TIP]
>
> try using one of these
> [![Robot player sprite preview](images/example-sprite-player-robot.png){:width="300px"}](images/example-sprite-player-robot.png)
>
> [![Adventurer player sprite preview](images/example-sprite-player-adventurer.png){:width="300px"}](images/example-sprite-player-adventurer.png)
>
> [![Creature player sprite preview](images/example-sprite-player-creature.png){:width="300px"}](images/example-sprite-player-creature.png)

## Step 3

> [!TASK]
>
> Select the **player** sprite in the sprite pane.
>
> ![Scratch Cat sprite selected in the sprite pain](images/player_sprite.png)

## Step 4

> [!TASK]
>
> Open the **Costumes** tab.
>
> ![The Costumes tab in Scratch.](images/tab_costumes.png)

## Step 5

> [!TASK]
>
> Open the costume menu and choose the **Upload Costume** icon.

## Step 6

> [!TASK]
>
> Select your player image from your computer. Scratch will add it as a new costume for the **player** sprite.

## Step 7

> [!TASK]
>
> Delete the **Cat-a** and **Cat-b** costumes.
>
> ![Two Scratch cat costumes in costumes pane](images/cat_costumes.png)
>

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
> Check that the **player** sprite shows your uploaded costume on the Stage. If it is too large, change the **Size** number in the sprite pane to make it smaller.
