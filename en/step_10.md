## 4A - Keys

Add keyboard controls so the **player** can run and jump.

## Step 1

> [!TASK]
>
> Select the **player** in the sprite pane.

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
> Add a `forever`{:class="block3control"} loop to your starting script and set `x speed`{:class="block3variables"} to `0`.
>
> ```blocks3
> when green flag clicked
> go to x: (-200) y: (-120)
> +forever
> set [x speed v] to (0)
> end
> ```

## Step 4

> [!TASK]
>
> Inside the `forever`{:class="block3control"} loop, add an `if`{:class="block3control"} block for moving right.
>
> If the `right arrow`{:class="block3sensing"} key is pressed, set `x speed`{:class="block3variables"} to `move speed`{:class="block3variables"} and point the **player** right.
>
> ```blocks3
> when green flag clicked
> go to x: (-200) y: (-120)
> forever
>   set [x speed v] to (0)
> +  if <key (right arrow v) pressed?> then
>     set [x speed v] to (move speed)
>     point in direction (90)
>   end
> end
> ```
>
> > [!TIP]
> >
> > If your **player** faces the wrong way, swap `90` with `-90`.

## Step 5

> [!TASK]
>
> Add another `if`{:class="block3control"} block for moving left, when the `left arrow`{:class="block3sensing"} key is pressed.
>
> This will set `x speed`{:class="block3variables"}. Use a `take away`{:class="block3operators"} block, with `0` in the first space and `move speed`{:class="block3variables"} in the second. Then point the **player** left.
>
> ```blocks3
> when green flag clicked
> go to x: (-200) y: (-120)
> forever
>   set [x speed v] to (0)
>
>   if <key (right arrow v) pressed?> then
>     set [x speed v] to (move speed)
>     point in direction (90)
>   end
>
> +  if <key (left arrow v) pressed?> then
>     set [x speed v] to ((0) - (move speed))
>     point in direction (-90)
>   end
> end
> ```

## Step 6

> [!TASK]
>
> At the bottom of the `forever`{:class="block3control"} loop, add `change x by (x speed)`{:class="block3motion"}.
>
> This moves the **player** by `x speed`{:class="block3variables"}: right when you press the right arrow, left when you press the left arrow, and not at all when no key is pressed.
>
> ```blocks3
> when green flag clicked
> go to x: (-200) y: (-120)
> forever
>   set [x speed v] to (0)
>
>   if <key (right arrow v) pressed?> then
>     set [x speed v] to (move speed)
>     point in direction (90)
>   end
>
>   if <key (left arrow v) pressed?> then
>     set [x speed v] to ((0) - (move speed))
>     point in direction (-90)
>   end
>
> +  change x by (x speed)
> end
> ```

## Test

> [!TASK]
>
> Click the green flag and use the arrow keys to move left and right.
>
> If the **player** moves too quickly or too slowly, change `move speed`{:class="block3variables"} in the starter setup script.
