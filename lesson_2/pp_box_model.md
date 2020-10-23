1. Given the code below, what is the minimum width and height (in pixels) that the div needs to entirely contain the img element (including its margins)?

    + height: 300 + 20 + 10 + 10 + 10 + 4 + 4 = 358 + 1 + 1 = 360
    + width: 500 + 19 + 11 + 20 + 20 + 4 + 4 = 578 + 1 + 1 = 580
    + answer = 580 x 360

2. Given the code below, what is the minimum width and height (in pixels) that the div needs to entirely contain the section element (including its margins)? How does this differ from the result of the previous practice problem?

    + height: 360
    + width: 580
    + answer: 580 X 360

      - The width and height is the same as the previous problem but the main difference is that the `section` in this problem will always be on a line by itself within the `div` no matter its width. 

3. Given the code below, what is the minimum width and height (in pixels) that the div needs to entirely contain the em element (including its margins)?

    + This depends on the width and height of the content since the `em` element is `inline` for the `display` property. The `div` is using `box-sizing` so its minimum width and height will be whatever the width and height of the `em` element. 

4. Given the code below, what is the minimum width and height (in pixels) that the div needs to be to entirely contain the article element (including its margins)?

    + width: 500 + 19 + 11 + 1 + 1= 532
    + height: 300 + 20 + 10 + 1 + 1= 332

    + Minimum width and height of `div` would have to be 532 x 332. Since `article` set the box-sizing property to `border-box`, we must ignore the padding and border to calculate the dimensions. 

5. Which of the following element pairs will display side-by-side in the <div>? Select all that apply:

    + 2. Both elements are inline elements.
    + 3. Both elements are inline-block elements.
    + 6. One element is an inline element, and one is an inline-block element.

6. Will the following code display the two article boxes side-by-side? If not, why not? How would you fix it so that it places the boxes side-by-side?


    + By default, `article` is a `block` element if the display property is not specifically defined so the two articles can't be side by side. 

    + To fix the code to make the two articles side by side, you have to add a `display` property equal to `inline-block` to the `article` element. Then add `box-sizing = border-box` to `article` as well so the border and padding is include in the 50% specified width for the `article` element. 

7. Challenge. Given our solution to the previous question, what will happen if we put the article tags on separate lines?

    + Since `article` is on two lines, the browser will see the whitespace (a newline and several spaces in this example) between the two articles. The broswer will collapse the whitespace into a single space character and use the results as content between the elements. With this additional "whitespace" content, the width is larger than 50% as specified in `article` so it will put the 2nd article on the 2nd line. You can fix this by changing the width property to 49% in `article`. 