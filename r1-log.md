# #100DaysOfCode Log - Round 1 - John M

The log of my #100DaysOfCode challenge. Started on [August 3rd, 2017].

## Log

### R1D1 20180803
#### freeCodeCamp

**Today's Progress:**
Note: Already on the _Basic CSS_ section since I actually started a few days ago.
- Maybe I already forgot this but I learned that an `id` has a higher specificity than a `class`. Since there's no code to push, here's my 100 day commitment [post](https://twitter.com/johnmmweb/status/1025618060483280896).
- Learned about another custom CSS selector (and it's syntax) by styling the margin around a checkbox.
```CSS
  [type='checkbox'] {
    margin: 10px 15px 10px 15px;
  }
```
- I knew about the `px`, percentage `%` and `em` measurements but I either forgot about or didn't know about the `in` and `mm` options I could use.

**Thoughts:** While I could fly through this CSS stuff, I'm trying to take it slower so hopefully some of this stuff will sink in deeper.

**Link to work:** No code yet. Working on the basics still. Here's my Twitter [post]().

#### Bloc.io
**Today's Progress**
- Completed the Data Structures checkpoint number 1.
- Learned more about stacks and queues.
- I'm jumping around between the data structures, algorithms and relational db fundamentals modules. I started reading checkpoint 10 of the db module which discusses normalization and denormalization.

**Thoughts:** Learned that classes are a way to structure [abstract data types](https://en.wikipedia.org/wiki/Abstract_data_type). I'm still hazy on how Ruby classes are formed and when to do initialization and when to make methods private.

**Link to work:**
Here's the latest [repo](https://github.com/jmuldvp/bloc-data-structures) for my data structures work.<br />

### R1D2 20180804
#### freeCodeCamp

**Today's Progress:**
Covered more and completed freeCodeCamp CSS basics.

**Thoughts:**
- Learned that whatever comes last in the CSS file is what takes precedence. Within the HTML, it doesn't matter what the order is but it does within the `<style>` tags or the CSS file and the browser reads CSS from top to bottom. Based on my note from yesterday, an `id` attribute will over ride both classes. An inline entry will over ride the `class` and `id` declarations. When other CSS libraries over ride your style, there is one last thing that trumps them all. Insert `!important` at the end of the line.
- Custom css variable `--left-navbar: gray`.
- When using custom variable `var(--left-navbar, black)` will default to gray but revert to black if there are issues.
- Because of cascading, CSS variables are often defined in the `:root` element.

**Link to work:**
No code on GitHub yet since all work is on on freeCodeCamp site still. Here's the Twitter [post](https://twitter.com/johnmmweb/status/1025807349989036033).

#### Bloc.io

**Today's Progress:**
Learned about data normalization.  Will pick up with denormalization next time.

**Thoughts:**
- Process of normalization is data should be divided into separate tables to *eliminate duplication*.
- >Normalization involves discarding repeating groups, minimizing redundancy, eliminating composite keys for partial dependency, and separating non-key attributes. Essentially, each attribute or column must be a fact about the key and nothing but the particular key. And each table should describe only one type of entity – for example a person, place, customer order, or product item.
- Benefits of normalization include data integrity, optimized queries, faster index creation and sorting, faster update performance and improved concurrency resolution. The improved concurrency part is about table locks affecting less data.
- 1NF = First normal form states that a column of a table cannot contain multiple values.
- 2NF = Second normal form states that the table must first be in 1NF. Second,  _all non-key attributes cannot be dependent on a subset of the primary key._
- 3NF = This first requires the table to be in 2NF. Second, _all transitive functional dependencies of non-prime attributes must not exist._
- Boyce Codd normal form (BCNF) = Before analysis can be done, 3NF must exist. Then _as well as for every dependency X -> Y, X must be a super key of the table. A super key is a set of attributes within a table whose values can be used to uniquely identify all other attributes._
- Disadvantages of a normalized db: It's not easy designing a 3NF db. If devs don't truly understand the various normalization steps, this can cause data anomalies and inconsistency. Queries can get pretty complex. This will also increase the need for more joins among more tables. Performance gets increasingly slower as the normal form progresses.

**Link to work:**
No code pushed today. Twitter post is [here](https://twitter.com/johnmmweb/status/1025807349989036033). <br />


### R1D3 20180806
#### freeCodeCamp

**Today's Progress:**
Half way through Applied Visual Design in freeCodeCamp.

**Thoughts:**
- `text-align: justify;` > causes all lines of text except the last line to meet the left and right edges of the line box. This goes to show how little I've played with laying out the front end but I didn't know what justify meant until now.
- All the options on `box-shadow` will be confusing until I have a chance to use it more than a handful of times. The options are `offset-x`, `offset-y`, `blur-radius`, `spread-radius` and finally color.
- This could come in handy for a navbar...  `text-transform: uppercase;`
- CSS box model = Block level items are headings, paragraphs or divs). Inline items are images and spans. This is called _normal flow_.
- > Hue is what people generally think of as 'color'.
- > Saturation is the amount of gray in a color.
- > Lightness is the amount of white or black in a color.

**Link to work:**
No code to push in this part. See Twitter [post](https://twitter.com/johnmmweb/status/1026712558638526464).

#### Bloc.io

**Today's Progress:**
Half way through the assignment.  Will push tomorrow night to GitHub.

**Thoughts:**
- > If data normalization aims to reduce redundancy, data denormalization is a process performed on a previously-normalized database to increase *read performance*. This happens at the expense of losing some write performance, by adding redundant copies of data or by grouping data.
- Methods of denormalization..
  1. Adding redundant groups
  2. Adding derived columns
  3. Combining tables
  4. Repeating groups
  5. Creating extract tables
  6. Partitioning relations
- Super key = a set of attributes within a table whose values can be used to uniquely identify all other attributes.


**Link to work:**
See Twitter [post](https://twitter.com/johnmmweb/status/1026712558638526464) for now.
<br />


### R1D4 20180807
#### freeCodeCamp

**Today's Progress:**
Almost finished the 'Applied Visual Design' section.  I should be finished with it tomorrow.

**Thoughts:**
- Learned about `background: linear-gradient(gradient_direction, color 1, color 2, color 3, ...);`. `rgb()` or `hsl()` could also be used in the color options. I'm not a CSS buff but I've been through a lot of tutorials and hadn't heard of that before.
- This is probably my inexperience talking but I just learned about `repeating-linear-gradient()` but I don't see any use for it unless the goal was to make a web page that looks like it was made in the 90's.  I'll have to google that to see if any big sites are using it and if so, how.
- Here's another I just learned about...  `background: url()` where the address is inserted in within the parentheses.
- `transform:scale(2);` makes something twice as big as it's normal size.
- By using `:hover` and `transform: scale(1.1)` will scale the object when the mouse hovers.
- `transform: skewX(24deg);` can change a rectangle to something looks like a parallelogram. `transform: skewY(-10deg);` can do the same but it moves it along the y-axis.
- Implementing an animation with `@keyframes` was kind of cool but would have to be used in moderation to keep a web page looking cool if used.
```
#anim {
  animation-name: colorful;
  animation-duration: 3s;
}
@keyframes colorful {
  0% {
    background-color: blue;
  }
  100% {
    background-color: yellow;
  }
}
```

**Link to work:**
No code to push for freeCodeCamp. See Twitter [post](https://twitter.com/johnmmweb/status/1027056646722281472) for update.

#### Bloc.io

**Today's Progress:**
- Completed checkpoint 10 (Data Normalization and Denormalization)
- Took the normalization-denormalization SQL quiz and passed it 11/12 the first time then 12/12 the next.
- I read the entire Stacks and Queues checkpoint... FIFO, LIFO and The Stack. Tomorrow I'll work on the assignment.

**Thoughts:**
- Flattened out the student_records table to 3NF.
- Assigning myself a personal task...I want to do that exercise but by putting students and professors in a person table.

**Link to work:**
[Link](https://github.com/jmuldvp/bloc-rdbf/blob/cp10-assign/cp10/cp10.md) the the markdown file containing the questions I had to answer. Also, see Twitter [post](https://twitter.com/johnmmweb/status/1027056646722281472).<br />

### R1D5
#### freeCodeCamp

**Today's Progress:**

**Thoughts:**

**Link to work:**

#### Bloc.io

**Today's Progress:**

**Thoughts:**

**Link to work:**
<br />

### R1D6
#### freeCodeCamp

**Today's Progress:**

**Thoughts:**

**Link to work:**

#### Bloc.io

**Today's Progress:**

**Thoughts:**

**Link to work:**
<br />
