## 4C - Always Moving

Make the **player** keep moving, and use the arrow keys to change direction.

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

The starter project already includes the `x speed`{:class="block3variables"} and `move speed`{:class="block3variables"} variables you will need.

## Step 3

> [!TASK]
>
> Set `x speed`{:class="block3variables"} to `move speed`{:class="block3variables"}, then add a `forever`{:class="block3control"} loop to start the **player** moving.
>
> ```blocks3
> when green flag clicked
> go to x: (-200) y: (-120)
> +set [x speed v] to (move speed)
> +forever
> change x by (x speed)
> end
> ```

## Step 4

> [!TASK]
>
> At the moment the **player** will always move to the right. 
>
> Add an `if`{:class="block3control"} block so that the **player** changes speed and direction when the `left arrow`{:class="block3sensing"} key is pressed.
> 
> ```blocks3
> when green flag clicked
> go to x: (-200) y: (-120)
> set [x speed v] to (move speed) 
> forever
> +if <key (left arrow v) pressed?> then
> point in direction (-90)
> set [x speed v] to ((0)-(move speed))
> end
> change x by (x speed)
> end
> ```
>
> > [!TIP]
> >
> > If your **player** faces the wrong way, swap `90` and `-90`.

## Step 5

> [!TASK]
>
> Add another `if`{:class="block3control"} block to change direction back again when the `right arrow`{:class="block3sensing"} key is pressed.
> 
> ```blocks3
> when green flag clicked
> go to x: (-200) y: (-120)
> set [x speed v] to (move speed) 
> forever
> if <key (left arrow v) pressed?> then
> point in direction (-90)
> set [x speed v] to ((0)-(move speed))
> end
> +if <key (right arrow v) pressed?> then
> point in direction (90)
> set [x speed v] to (move speed)
> end
> change x by (x speed)
> end
> ```

## Test

> [!TASK]
>
> Click the green flag and check the arrow keys change the direction.
>
> You can change the value of `move speed`{:class="block3variables"} if you want the sprite to move faster or slower.
