autoscale: true
footer: © New York Code + Design Academy 2016
slidenumbers: true

# jQuery DOM Manipulation Extended

---

# What else can jQuery do with the DOM?
Quite a bit, you'll see.

You can change styles, move things, hide them, or remove them completely. We're going to explore some of it now just to get some familiarity, but the options are almost endless!

---

# Animation

Let's say you want a div to grow larger when you hover over it, you know, for professional effect. You could do this:
```JS
$('#some-div').hover(function(){
  $(this).animate({
    width: "+=200"
  });
});
```
##### Try it now!

---

# Oh dear...

That div just keeps getting bigger and bigger! That's not what we want.
We would rather restore its width when we aren't hovering over it anymore, right?

Let's talk about jQuery's amazing ability called chaining events.

```JS
$('#some-div').mouseenter(function(){
  $(this).animate({
    width: '+=200'
  })
  .mouseout(function(){
    $(this).animate({
      width: '-=200'
    });
  });
});
```
That's pretty sweet, huh? Let's break this down on the next slide.

---
# The Breakdown
```JS
$('#some-div') //Selects the div
```

---
# The Breakdown

```JS
//Adds a mouseenter event to the div
$('#some-div').mouseenter(function(){
  $(this).animate({
    width: '+=200'
  })
```

---
# The Breakdown

```JS
//With chaining, jQuery adds the event to the originally selected div!
$('#some-div').mouseenter(function(){
  $(this).animate({
    width: '+=200'
  })
  .mouseout... //mouseout event added to #some-div
```

---

# Exercise

Try out your new chaining skills by hiding a div on mouseenter and showing it again on mouseout.

_Hint: Google 'jQuery hide' and 'jQuery show'_

---

# Keypress

Let's say you have an input box and you want whatever is typed into it to show up in the div next to it. With jQuery, that's simpler than sneezing!

```HTML
<div>
  <input id="letters" type="text" name="letters">
  <div id="show-letters">
    <!-- Where the letters will show -->
  </div>
</div>
```
```JS
$('#letters').keyup(function(){
  $('#show-letters').text($(this).val());
});
```
Let's break this down on the next slides
---

# The Breakdown

```JS
//Adds a listener for when a keyup event
$('#letters').keyup(...);
```
---

# The Breakdown

```JS
  //
  $('#show-letters').text(/*text we want to put in div*/);
```

---

# The Breakdown

```JS
  $('#show-letters').text($(this).val());
  //$(this) = input with id="letters"
  //.val() gets the value of the input
```
So this is setting the text of the div to be the text that is the value of the input!
Woah, you might want to read that a few more times to get that.
