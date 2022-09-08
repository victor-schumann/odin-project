# Flexbox Lesson Notes

<!--
<div><details>
<summary>
<b>How </b>
</summary>

a
</details></div>
-->

<div><details>
<summary>
<b>1. How to init a flex container?</b>
</summary>

``display: flex;``
</details></div>


<div><details>
<summary>
<b>2. How to define the horizontal or vertical alignment of flex-items?</b>
</summary>

``justify-content: ______;`` 
``align-items: ______;``
</details></div>


<div><details>
<summary>
<b>3. How to switch from rows to columns configuration? And how do we use the same property to invert the order?</b>
</summary>

``flex-direction: column;``
``flex-direction: column-reverse;``
``flex-direction: row-reverse;``

Notice that (when we switch to columns) the column is hugging the left side of its flex container despite our justify-content: center; declaration. When you rotate the direction of a container, you also rotate the direction of the justify-content property. It now refers to the container’s vertical alignment—not its horizontal alignment.
>
<img alt="Visual representation of the 'flip' of orientation" width="400" src="images/flex-direction.png"/></div>

</details></div>

<div><details>
<summary>
<b>4. How to customize the position of individual elements?</b>
</summary>

``order: 1;`` -> or 2, or 3...
``order -1;`` -> or -2, or -3...
</details></div>

<div><details>
<summary>
<b>5. How to customize the vertical position of individual elements?</b>
</summary>

``align-self: flex-end;`` (bottom)
``align-self: flex-start;`` (top)
</details></div>

<div><details>
<summary>
<b>6. How to create flexible boxes that can stretch and shrink based on "fixed" boxes?</b>
</summary>

On the main class, let's set a ``flex: 1;`` and on the child, we make sure to add ``flex: initial;`` followed by a given height or width definition. That will fix them while the other(s) inherit the ``flex: 1;``, allowing them to, well, flex.

<img alt="Visual representation of the selective stretching of flex items" width="400" src="images/flex-init.png"/></div>
</details></div>