## 2C - Choose Inbuilt Player

Choose a costume from the Scratch library for the existing **player** sprite in the starter project.

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

## Step 3

> [!TASK]
>
> Open the **Costumes** tab.
>
> ![The Costumes tab in Scratch.](images/tab_costumes.png)

## Step 4

> [!TASK]
>
> Open the costume menu and select **Choose a Costume**.
>
> ![The costume library in Scratch.](images/list-costume.png)

## Step 5

> [!TASK]
>
> Pick a costume from the Scratch library. Choose one that is clear, easy to see, and a good fit for the world of your platformer.
>
> For a classic platformer, a costume with legs, wheels, or a clear body shape is usually easier to understand as the player.

## Step 6

> [!TASK]
>
> Add the costume to the **player** sprite. If the **player** already has another costume, keep it because you may be able to use it for an animation later.
>
> > [!TIP]
> >
> > Some Scratch library sprites with multiple costumes need you to add each costume one at a time. For example, **Unicorn** and some walking sprites need their individual costumes added separately.

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
> Check that the **player** sprite shows your chosen costume on the Stage and is easy to see against your backdrop.
