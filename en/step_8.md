## 3B - Draw foreground platforms

Draw visible foreground platforms in one **platform** sprite so the **player** has places to stand and jump.

## Step 1

> [!TASK]
>
> Open the **Choose a Sprite** menu and select **Paint**.
>
> ![The Paint option in the Choose a Sprite menu.](images/sprite-paint.png)

## Step 2

> [!TASK]
>
> In the **platform** sprite, draw a block that spans the entire lower edge of the Stage.
>
> This is the floor. It gives the **player** solid ground to stand on and stops them falling off the bottom of the Stage.
>
> Give the floor a straight, horizontal top.

## Step 3

> [!TASK]
>
> Draw the foreground platforms in the **platform** sprite.
>
> The place where the **player** stands must have a straight, horizontal top.
>
> Draw every platform for the level in this one sprite.
>
> > [!TIP]
> >
> > You can also copy and paste platform images into the paint editor, then arrange them where you want them.
> >
> > If you paste an image, crop or delete any empty pixels around it so the artwork fits tightly around the platform.

## Step 4

> [!TASK]
>
> In the sprite pane, change the sprite name to **platform**.
>
> Use this exact spelling so later steps can check whether the **player** is touching the **platform** sprite.

## Step 5

> [!TASK]
>
> Put the **platform** sprite in the centre of the Stage.
>
> The foreground platform drawings should match the places where you want the **player** to stand.

## Step 6

> [!TASK]
>
> Open the **Code** tab.
>
> ![The Code tab in Scratch.](images/code-tab.png)

## Step 7

> [!TASK]
>
> Add a green flag block.
>
> ```blocks3
> +when green flag clicked
> ```

## Step 8

> [!TASK]
>
> Add blocks to show the **platform** sprite, move it to the front layer, put it in the centre of the Stage, and set its size.
>
> ```blocks3
> when green flag clicked
> +show
> +go to [front v] layer
> +go to x: (0) y: (0)
> +set size to (100)%
> ```

## Test

> [!TASK]
>
> Click the green flag and check that the foreground platforms appear in front of the backdrop in the places you chose.
>
> The **player** should be able to stand or jump on each foreground platform.
