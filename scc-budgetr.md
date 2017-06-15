autoscale: true
footer: © New York Code + Design Academy 2017
slidenumbers: true

# Project: Budgetr
---

# So you're adulting now, right?

While adulting, you will need to budget your monies so that you don't end up with more month than monies. There are lots of budgeting systems out here, but you are about to make the best because, well, you made it!

#### Goal
To learn more familiarity with jQuery, Javascript, HTML, and CSS

Guidelines for how it will look:
  - Make the page so that all the content is inside a fixed width div (meaning there is spacing on either side of the content)
  - Give some user feedback, like color changes on hover, the progress bar doesn't update too fast, etc.

It will do the following:
  - You will have categories to budget for
    - Each category will have two input boxes: one for the budgeted amount, and one for the spent amount
      - These are hidden until a user clicks something to show them and then clicks again to hide
    - There will be a progress bar in each category that shows the percentage of that budget spent and adjusts when the numbers change
      - The progress bars will change color to indicate under spent, almost spent the whole budgeted amount, or over spent
          - Green when spent < 90% of budgeted
          - Yellow when spent > 90% and < 100% of budgeted
          - Red when spent > 100% of budgeted
  - Have a fixed position summary box on one side (like in Mint) that shows the total budgeted amount, the total spent amount, and indicates if you have overspent.
