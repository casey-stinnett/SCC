# HTML Structure for CSS

---

# There's HTML, then there's CSS
### Then there's HTML built for easier CSS
Knowing HTML is one thing. CSS is another. But how do you get them to play well together?

---
# HTML for CSS Positioning
Let's say for example you want something like this:
![Screen Shot 2017-05-01 at 4.30.17 PM](</assets/Screen Shot 2017-05-01 at 4.30.17 PM.png>)

There are logical groupings that make sense to keep by one another.
For example, each eye needs to be grouped with an eye brow.
And each eye needs to be under the eye brow. So we need them to be together and they are placed relative to each other. So it would make sense to group them together, right?

---
# Face Groupings

![Screen Shot 2017-05-01 at 4.35.34 PM](</assets/Screen Shot 2017-05-01 at 4.35.34 PM.png>)

Above are the logical groupings outlined.
The idea is, if you need elements to move together, then group them in a parent element!

---
# HTML View

```HTML
<!-- Face Wrapper -->
<div class="face">
  <!-- Left Eye Wrapper -->
  <div class="left-eye">
    <div class="eye-brow"></div>
    <div class="eye-ball"></div>
  </div>
  <!-- Right Eye Wrapper -->
  <div class="right-eye">
    <div class="eye-brow"></div>
    <div class="eye-ball"></div>
  </div>
  <!-- Mouth Area Wrapper -->
  <div class="mouth-area">
    <div class="nose"></div>
    <div class="stache"></div>
    <div class="mouth"></div>
  </div>
</div>
```
Any wrapper you move, moves its children as well!

---


# So do I have to set up my HTML first and then make the CSS match or vice versa?

### It's back and forth, really.

Well, the longer you code, the more you'll realize that when to do the HTML, CSS, or JS is really up in the air. You set up some HTML, you do some CSS, you adjust some HTML to match your CSS, etc. It's back and forth, really.

---
