# CSS
CSS practical skills
### 1. CSS Selectors
 |selector            |level
 |:------------------:|------------------------------------|
 | *                  |0
 | p                  |1(one element)
 | li:first-of-type   |2(one element, one pseudo-element)
 | ul li              |2(two elements)
 | ul ol+li           |3(three elements)
 | h1+*[href*=index]  |11(one attribute,one element)
 | ul ol li.list-item |13(one class,three elements)
 | <p style=""></p>   |1000(one inline styling)
 | .class             |10(one class selector)
 | div p.class        |12(two element selectors and one class selector)
 |#id                 |100(one id selector)
### 2. avoid using !important
If someone used !important in CSS style sheet, you want to avoid its impact. Only things you could do are either to remove !important before you are absolutly sure this removement can't make everything messed up, or use higher level CSS selectors. First one takes time. 
The worst is that this problem cannot be fixed. Another following developer has to use more complex selector to make it work.
### 3. Don't use ID
If you want a diverse style, don't use ID. ID can't be reused.One element with diverse style need many ID and relative CSS to make it work.
ID is better in JS!
### 4. avoid using complex selectors
browser will read css one by one from the right to the left. Complex selectors will make render slower.
### 5. reset css
Why? 
Different browser render css differently. Reset default css for these elements can fix it.
How?
Do it your self or using some style sheets(Normalize.css/Reset.css)

https://github.com/necolas/normalize.css/
### 6. Dont't reset css for all elements!
