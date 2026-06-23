## 8B - Target Score

Make the player win when their **Score** reaches a target value.

## Step 1

> [!TASK]
>
> Make sure you have a variable called `Score`.
>
> Set it up for **all sprites** so the Stage and other sprites can use it.
>
> > [!TIP]
> >
> > A target score only works if something makes `Score` go up as the player plays, and collectables are the perfect basis for a scoring system. If you have not added any yet, it is well worth going back to `Place Collectables` or `Random Collectables` and adding them first. Each collectable the player touches adds `1` to `Score`, giving this step a value to count towards.

## Step 2

> [!TASK]
>
> Select the **Stage** and add a script that starts when the green flag is clicked.
>
> ```blocks3
> +when green flag clicked
> ```

## Step 3

> [!TASK]
>
> Add a block to set `Score` to `0`.
>
> ```blocks3
> when green flag clicked
> +set [Score v] to (0)
> ```

## Step 4

> [!TASK]
>
> Add a `forever`{:class="block3control"} loop below the variable setup block.
>
> ```blocks3
> when green flag clicked
> set [Score v] to (0)
> +forever
> +end
> ```

## Step 5

> [!TASK]
>
> Inside the `forever`{:class="block3control"} loop, add an `if`{:class="block3control"} block that checks whether `Score` has reached your target value.
>
> This example checks whether `Score` is `5` or more.
>
> ```blocks3
> when green flag clicked
> set [Score v] to (0)
> forever
> +  if <(Score) > (4)> then
> +  end
> end
> ```

## Step 6

> [!TASK]
>
> Inside the `if`{:class="block3control"} block, add `broadcast win`{:class="block3events"}.
>
> ```blocks3
> when green flag clicked
> set [Score v] to (0)
> forever
>   if <(Score) > (4)> then
> +    broadcast (win v)
>   end
> end
> ```

## Step 7

> [!TASK]
>
> Add a new script that starts when it receives the `win`{:class="block3events"} message.
>
> Add `say 'You win!' for 2 seconds`{:class="block3looks"} and `stop all`{:class="block3control"}.
>
> If you already added this win script in another route, just check this step off.
>
> ```blocks3
> +when I receive [win v]
> +say [You win!] for (2) seconds
> +stop [all v]
> ```

## Step 8

> [!TASK]
>
> Choose what should happen before `stop all`{:class="block3control"}.
>
> You can use the `when I receive win`{:class="block3events"} script to show a message, play a sound, change backdrop, switch costume, or trigger another sprite before the game stops.
>
> Put any extra win blocks above `stop all`{:class="block3control"}.

## Test

> [!TASK]
>
> Play your game and increase `Score`.
>
> Check that the `win`{:class="block3events"} message broadcasts when `Score` reaches the target value, the win message appears, and the game stops.
