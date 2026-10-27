## 4B - Mouse Move

Make the **player** follow the mouse on the x-axis.

## Step 1

> [!TASK]
>
> Select the **player** sprite in the sprite pane.

## Step 2

> [!TASK]
>
> Open the **Code** tab.
>
> ![The Code tab in Scratch.](images/code-tab.png){:width="450px"}

The starter project already includes the `x speed`{:class="block3variables"} variable you will need.

## Step 3

> [!TASK]
>
> Inside a `forever`{:class="block3control"} loop, point the **player** at the mouse-pointer.
>
> ```blocks3
> when green flag clicked
> go to x: (-200) y: (-120)
> +forever
> point towards (mouse-pointer v)
> end
> ```

## Step 4

> [!TASK]
>
> The **player** sprite is going to move towards the mouse-pointer, but only left and right.
>
> ```blocks3
> when green flag clicked
> go to x: (-200) y: (-120)
> forever
> point towards (mouse-pointer v)
> +set [x speed v] to ((mouse x) - (x position))
> +change x by (x speed)
> end
> ```

## Test

> [!TASK]
>
> Click the green flag and move the mouse left and right.
>
> The sprite should always be at about the same x position as the mouse-pointer.
>
> This motion is probably a little too fast

## Step 5

> [!TASK]
>
> Slow the sprite down by dividing its speed by `10`
>
> ```blocks3
> when green flag clicked
> go to x: (-200) y: (-120)
> forever
> point towards (mouse-pointer v)
> +set [x speed v] to (((mouse x) - (x position)) / (10))
> change x by (x speed)
> end
> ```
>
> If this is too fast or too slow, you can choose a number larger or smaller than `10`.
