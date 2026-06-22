## 5B - Player Jump-Fall (Mouse)

Make your **player** sprite jump.

## Step 1

> [!TASK]
>
> Select the **player** sprite and find the mouse movement blocks you made earlier.

## Step 2

> [!TASK]
>
> Add in a new `if`{:class="block3control"} block, below the others, but above the `change x by ()`{:class="block3motion"} block.
>
> ```blocks3
> when green flag clicked
> go to x: (-200) y: (-120)
> forever
> point towards (mouse-pointer v)
> set [x speed v] to (((mouse x) - (x position)) / (10))
> +if <> then
> +end
> change x by (x speed)
> end
> ```

## Step 3

> [!TASK]
>
> Detect mouse clicks in `if`{:class="block3control"} and then change the `y speed`{:class="block3variables"} of the **player**.
>
> ```blocks3
> when green flag clicked
> go to x: (-200) y: (-120)
> forever
> point towards (mouse-pointer v)
> set [x speed v] to (((mouse x) - (x position)) / (10))
> +if <mouse down?> then
> +set [y speed v] to (jump strength)
> end
> change x by (x speed)
> end
> ```

## Test

> [!TASK]
>
> Click the green flag and click the mouse to jump
>
> If you click several times, then the sprite will jump "double-jump".

## Step 4

> [!TASK]
>
> If you don't want to enable double-jumps, then jumping should only work when the sprite is on the ground. There's an `on ground`{:class="blocks3variables"} to detect this.
>
> ```blocks3
> when green flag clicked
> go to x: (-200) y: (-120)
> forever
> point towards (mouse-pointer v)
> set [x speed v] to (((mouse x) - (x position)) / (10))
> +if <<mouse down?> and <(on ground) = (1)>> then
> set [y speed v] to (jump strength)
> end
> change x by (x speed)
> end
> ```

## Test

> [!TASK]
>
> Click the green flag and click several times. The **player** should only jump once.

## Step 5

> [!TASK]
>
> Change the height the **player** can jump and the speed that it falls, by changing the `gravity`{:class="block3variables"} and `jump strength`{:class="block3variables"} variables.
>
> ```blocks3
> set [gravity v] to (-1)
> set [jump strength v] to (15)
> ```

## Test

> [!TASK]
>
> Click the green flag and test your jump height.
>
> Make sure the **player** can jump high enough to land on the platforms above, but not so high that it shoots off the top of the Stage.
>
> Adjust the `jump strength`{:class="block3variables"} and `gravity`{:class="block3variables"} variables until the **player** can move between all of your platforms properly.
