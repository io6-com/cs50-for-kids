# 算法

* So now we can represent inputs and outputs. The black box earlier will contain _algorithms_, step-by-step instructions for solving a problem: ![box with word &quot;algorithms&quot;](https://cs50.harvard.edu/college/notes/0/algorithms.png)
* Let’s say we wanted to find a friend, Mike Smith, in a phone book.
  * We could start by flipping through the book, one page at a time, until we find Mike Smith or reach the end of the book.
  * We could also flip two pages at a time, but if we go too far, we’ll have to know to go back a page.
  * But an even more efficient way would be opening the phone book to the middle, decide whether Mike will be in the left half or right half of the book \(because the book is alphabetized\), and immediately throw away half of the problem. We can repeat this, dividing the problem in half each time. With 1024 pages to start, we would only need 10 steps of dividing in half before we have jsut one page remaining to check.
* In fact, we can represent the efficiency of each of those algorithms with a chart: ![chart with: &quot;size of problem&quot; as x-axis; &quot;time to solve&quot; as y-axis; red, steep straight line from origin to top of graph labeled &quot;n&quot;; yellow, less steep straight line from origin to top of graph labeled &quot;n/2&quot;; green, curved line that gets less and less steep from origin to right of graph labeled &quot;log n&quot;](https://cs50.harvard.edu/college/notes/0/running_time.png)
  * Our first solution, one page at a time, is like the red line: our time to solve increases linearly as the size of the problem increases.
  * The second solution, two pages at a time, is like the yellow line: our slope is less steep, but still linear.
  * Our final solution, is like the green line: logarithmic, since our time to solve rises more and more slowly as the size of the problem increases. In other words, if the phone book went from 1000 to 2000 pages, we would need one more step to find Mike. If the size doubled again from 2000 to 4000 pages, we would still only need one more step.

