# 数据表示

光会数数，那计算机不就只是个计算器了吗？数字我们知道在计算机中怎么表示了，那么文字，图片，视频，还有声音呢？

## 文字

* To represent letters, all we need to do is decide how numbers map to letters. Some humans, many years ago, collectively decided on a standard mapping called [ASCII](https://en.wikipedia.org/wiki/ASCII). The letter “A”, for example, is the number 65, and “B” is 66, and so on. The mapping also includes punctuation and other symbols. Other characters, like letters with accent marks, and emoji, are part of a standard called [Unicode](https://en.wikipedia.org/wiki/Unicode) that use more bits than ASCII to accommodate all these characters.
  * When we receive an emoji, our computer is actually just receiving a decimal number like `128514` \(`11111011000000010` in binary, if you can read that more easily\) that it then maps to the image of the emoji.

## 图片

* An image, too, is comprised of many smaller square dots, or pixels, each of which can be represented in binary with a system called RGB, with values for red, green, and blue light in each pixel. By mixing together different amounts of each color, we can represent millions of colors: ![red square labeled with 72, green square labeled with 73, blue square labeled with 33](https://cs50.harvard.edu/college/notes/0/rgb.png)
  * The red, green, and blue values are combined to get a light yellow color: ![light yellow square](https://cs50.harvard.edu/college/notes/0/rgb_combined.png)
* We can see this in an emoji if we zoom in far enough: ![zoomed-in emoji of laughing tears of joy with squares of pixels distinguishable](https://cs50.harvard.edu/college/notes/0/emoji_zoomed.png)

## 视频

* And computer programs know, based on the context of its code, whether the binary numbers should be interpreted as numbers, or letters, or pixels.
* And videos are just many, many images displayed one after another, at some number of frames per second. Music, too, can be represented by the notes being played, their duration, and their volume.

## 声音

声音blabla

