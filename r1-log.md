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

### R1D5 20180808
#### freeCodeCamp

**Today's Progress:**

I wasn't able to get to do any of the freeCodeCamp camp material.  I spent the last 5 hours working on a Stacks and Queue's assignment.

#### Bloc.io

**Today's Progress:**
I was able to get spec tests to pass for a Ruby stack exercise but I'm having problems with implementing a `pop` function without using the actual `pop` function.  Per the assignment, I'm not supposed to use that function.
Hopefully I'll be able to finish this checkpoint tomorrow.

**Thoughts:**
- Stack = This is like LIFO.  When you stack papers on top of each other, you pick the top one off the pile when you need to use it or move it.
- Queue = This is like FIFO.  This is like a line at the grocery store. First one in the line is the first out.

**Link to work:**
See Twitter [post](https://twitter.com/johnmmweb/status/1027419894210428928).
<br />

### R1D6 20180909
#### freeCodeCamp

**Today's Progress:**
I completed the Applied Visual Design section of CSS.

**Thoughts:**
- I'm used to using numbers to set values in CSS but just learned about the word `infinite` that can be used in `animation-iteration-count`.
- Note on `cubic-bezier`.
> cubic-bezier(0.3, 0.4, 0.5, 1.6);
> Notice that the value of y2 is larger than 1. Although the cubic Bezier curve is mapped on an 1 by 1 coordinate system, and it can only accept x values from 0 to 1, the y value can be set to numbers larger than one. This results in a bouncing movement that is ideal for simulating the juggling ball.

- I think there could be a whole course on CSS applied visual design.  There's too much to know about this. I'm proceeding through these CSS sections just to get the basics. My goal is not to get involved too much in UX.

**Link to work:**
See Twitter [post](https://twitter.com/johnmmweb/status/1027777902497083392).

#### Bloc.io

**Today's Progress:**
Completed the Stacks and Queue's assignment

**Thoughts:**
- I feel dumb getting stuck on what I feel are easy things.  One line messed me up on the mystack.rb coding exercise.

**Link to work:**
Here's my [work](https://github.com/jmuldvp/bloc-data-structures/tree/cp2-assign) for this assignment.

<br />

### R1D7 20180810
#### freeCodeCamp

**Today's Progress:**
I'm almost half way through the *Applied Accessibility* challenges.

**Thoughts/Notes:**
- I didn't know that the `alt` tag was looked at by search engines. Note to self, always use `alt` tags on images.
- I never knew this... > One final point, each page should always have one (and only one) h1 element, which is the main subject of your content. This and the other headings are used in part by search engines to understand the topic of the page.
- Tag names like `main`, `header`, `footer`, `nav`, `article` and `section` > ..can indicate the type of information it contains, which adds semantic meaning to that content. Assistive technologies can access this information to provide better page summary or navigation options to their users.
- In the FCC challenge, the `main` tag goes between `header` and `footer`.
- The `article` tag is > ...a sectioning element, and is used to wrap independent, self-contained content. The tag works well with blog entries, forum posts, or news articles.
- <div> - groups content
<section> - groups related content
<article> - groups independent, self-contained content
- About the `header` tag.. > ...header is meant for use in the body tag of your HTML document. This is different than the head element, which contains the page's title, meta information, etc.
- The `nav` tag is meant to wrap around all the main navigation links.  However > ...If there are repeated site links at the bottom of the page, it isn't necessary to markup those with a nav tag as well. Using a footer is sufficient.
- The `footer` tag is > ...primarily used to contain copyright information or links to related documents that usually sit at the bottom of a page.

**Link to work:**
See Twitter [post](https://twitter.com/johnmmweb/status/1028161767522762753).

#### Bloc.io

**Today's Progress:**
Read through the *Linked Lists* checkpoint slowly to try and understand it as best as I can.

**Thoughts/Notes:**
- *Spatial Locality* = When cpu requests data no found in cache, it retrieves an entire range of locations in ram and places it in cache.
- There is no code in the check point but rather reading to understand concepts about *Linked Lists*.
  - Definition of a *Linked List* = >  data structure that permits the sequential order of elements, much like an Array, but it circumvents Array’s memory issues.
  - To maintain a linked list, code will store a reference to the first node in the list called the _head_.
  - Indexing a *Linked List* is not possible like it is with arrays. To access an element, you have to start at the beginning.
- While there was an explanation of the pros and cons of *Linked Lists* given, I'm still not understanding it. Not sure why every node in a *Linked List* being instantiated so that it never consists of empty placeholders is a good thing.  As far as the con is concerned, I'm still not sure what a 'Cache-miss' is.  

**Link to work:**
See Twitter [post](https://twitter.com/johnmmweb/status/1028161767522762753).
<br />

### R1D8 20180811
#### freeCodeCamp

**Today's Progress:**
Completed all of the applied accessibility challenges.

**Thoughts/Notes:**
- The `audio` tag is used with the `controls` attribute.
```
<audio id="meowClip" controls>
  <source src="audio/meow.mp3" type="audio/mpeg" />
</audio>
```
- Another tag that helps is `label`.  See example...
```
<form>
  <label for="name">Name:</label>
</form>
```
- Example of using `fieldset` and `legend`...
```
<form>
  <fieldset>
    <legend>Choose one of these three items:</legend>
    <input id="one" type="radio" name="items" value="one">
    <label for="one">Choice One</label><br>
    <input id="two" type="radio" name="items" value="two">
    <label for="two">Choice Two</label><br>
    <input id="three" type="radio" name="items" value="three">
    <label for="three">Choice Three</label>
  </fieldset>
</form>
```
- For `input` and letting a user pick a date, here is some sample code..
```
<label for="input1">Enter a date:</label>
<input type="date" id="input1" name="input1">
```
- Using the `time` element, here's an example...
```
<time datetime="2013-02-13">last Wednesday</time>
```
- The next sections talk about hsl and contrasting colors.  While I'm glad I read over it, I don't see myself need to use this information much since I'm going to be doing more backend work with the exception of a blog that I might start.  when I do that, I'm going to be choosing colors that really contrast with each other.
- This can help keyboard only users in choosing links..
```
<button accesskey="b">Important Button</button>
```
- Using the `tabindex` element also helps keyboard users.  If there is a negative number, it means that it's not keyboard accessible.
```
<div tabindex="0">I need keyboard focus!</div>
```
-

**Link to work:**
I hope to be able to have a Github link here sometime soon. Still going to use the Twitter [post](https://twitter.com/johnmmweb/status/1028474774089912320) for now.

#### Bloc.io

**Today's Progress:**
Started the *Linked Lists* assignment.

**Thoughts/Notes:**
- Looks like the idea is to learn how to use classes from other files as well as learning about the logic of linked lists.

**Link to work:**
No code pushed since I wasn't able to finish the assignment tonight.
<br />


### R1D9 20180813
#### freeCodeCamp

**Today's Progress:**
I did not work on freeCodeCamp material tonight.

#### Bloc.io

**Today's Progress:**
Still working on the assignment for data structures assignment for checkpoint 3

**Thoughts/Notes:**
- I finally got the RSpec test to pass for adding to the end of a linked list.  Now I'm having problems with removing an item from the end of the array.

**Link to work:**
See [my Twitter post](https://twitter.com/johnmmweb/status/1029240144002334720)
<br />

### R1D10 20180814
#### freeCodeCamp

**Today's Progress:**
Completed Responsive Web Design Principles

**Thoughts/Notes:**
- Started *Responsive Web Design Principles*
- Covered the `@media` tag.
- In this code...
```
img {
  max-width: 100%;
  display: block;
  height: auto;
}
```
The `max-width` tag scales the width to fit inside it's container. The `display` element changes it from an in-line element to a block element. The `height` element keeps the original aspect ratio.
- Completed Responsive Web Design Principles.  I can't wait to learn FlexBox.

**Link to work:**
See [Twitter post](https://twitter.com/johnmmweb/status/1029602300300410882)

#### Bloc.io

**Today's Progress:**
I figured out some issues I had in my understanding of linked lists but am still stuck on the exercise of getting the rspec tests to pass.

**Thoughts/Notes:**
- I misunderstood the material in the checkpoint so I'm having to refer to other material to get a grasp of what a linked list is.
- The node.rb file is there to create new nodes. At first I thought it was an array of arrays but after a discussion with a coach, it seemed like an array of hashes (key value pair) but instead its a collection of objects.

**Link to work:**
See [Twitter post](https://twitter.com/johnmmweb/status/1029602300300410882)
<br />

### R1D11 20180815
#### freeCodeCamp

**Today's Progress:**
Made it halfway through the CSS FlexBox challenges.

**Thoughts/Notes:**
- To activate FlexBox, use `display: flex;` at the top of the element.
- Using `flex-direction: row-reverse;` will reverse the elements.
- Using `flex-direction: row;` lines things up in a row.
- Using `flex-direction: column;` stacks the elements on top of each other.
- The `justify-content:` option allows you to evenly space things out.  The options that can be used with this are `center`, `flex-start`, `flex-end`, `space-between`, `space-around` and `space-between`.

**Link to work:**
See [the Twitter post](https://twitter.com/johnmmweb/status/1029958975343583232).

#### Bloc.io

**Today's Progress:**
`add_to_tail` method complete.  Now I'm stuck on the `remove_tail` method.

**Thoughts/Notes:**
- I thought I had a handle on how to work with linked lists but I was way off base.
- The code for adding a node to the tail of a list was a lot shorter than I thought.

**Link to work:**
No code to push yet.
<br />

### R1D12 20180816
#### freeCodeCamp

**Today's Progress:**
No progress on freeCodeCamp material today.

#### Bloc.io

**Today's Progress:**
Almost finished checkpoint 3.

**Thoughts/Notes:**
- Linked list is hard to understand but I feel I have even a better grasp of it now than I did yesterday.

**Link to work:**
Still working on the last benchmarking test to compare how fast using a linked list compared against an array.
<br />

### R1D13 20180817
#### freeCodeCamp

**Today's Progress:**
Still no further progress on freeCodeCamp.

#### Bloc.io

**Today's Progress:**
Completed the linked list assignment. Currently working through the first checkpoint in Engineering Principles - ORM Architecture.

**Thoughts/Notes:**
- After in SQLite3, `.tables` lists tables. `.databases` lists all of the db's. `.headers on` turns on the headers to keep the output of select statements organized. `.mode column` also helps with the look of the output.
- By default foreign keys are disabled.  Must make enter this to change that... `PRAGMA foreign_keys = ON;`  "pragma" is also known as a pragmatic directive.
- `.save data.db` saves the information out to a file.

**Link to work:**
Here's the [GitHub repo for my ORM studies](https://github.com/jmuldvp/orm-arch).
<br />

### R1D14 20180818
#### freeCodeCamp

**Today's Progress:**
Didn't get to this today.

#### Bloc.io

**Today's Progress:**

**Thoughts/Notes:**
- I thought the db would open with the tables I created from last time but I found out otherwise.
- New commands learned `.open "file name here"`.
- Learning ActiveRecord and it's finally starting to click.

**Link to work:**
<br />

### R1D15 20180820
#### freeCodeCamp

**Today's Progress:**
No progress on freeCodeCamp stuff today.

#### Bloc.io

**Today's Progress:**
Completed ORM checkpoint 1. I got halfway through the *Databases: Create an ORM* section of the ORM material.

**Thoughts/Notes:**
- Creating a new framework called *BlocRecord* which will be a drop-in replacement for ActiveRecord.  Advice given the the checkpoint...
> In a project deployed to real users, you should still use  ActiveRecord or a robust alternative like [DataMapper](http://datamapper.org/).

- Creating this project as a RubyGem, allows for integration with other software.
- At minimum, a RubyGem needs a _.gemspec_ file and one Ruby file.
- The gemspec file defines metadata about the RubyGem like name, version etc.
- A gemspec is called from a Ruby method.
- The plan is to add `BlocRecord` to `AddressBloc`.  This is a command-line address book app written in Ruby. In it's current form, the information is only saved when the app is running so it doesn't persist. The plan is to make it so that it does persist and keep the data.
- In the main file `lib/bloc_record.rb`, code is created to connect to the database...or rather call code from another file that allows it to connect.
- The file used to encapsulate the code for the connection is `bloc_record/connection.rb`.
- Creating 2 more files...
  - The first file `lib/bloc_record/utility.rb` will contain reusable functions for transforming data.
  - The second file `lib/bloc_record/schema.rb` will contain information about the database schema.
    - Methods added to the schema are *table*, *schema*, *columns*, *attributes* and *count*. The *count* method uses things I've seen before like a heredoc `<<-` that I first learned about in PHP and then it looks like an actual SQL statement.
    ```
    def count
      connection.execute(<<-SQL)[0][0]
        SELECT COUNT(*) FROM #{table}
      SQL
    end
    ```

    The code could have also been written this way...
    ```
    connection.execute("SELECT COUNT(*) FROM #{table}")[0][0]
    ```
    > However, our SQL queries will get longer and the best practice is to format with heredoc to separate the SQL query from the code.

**Link to work:**
I haven't completed the work on the checkpoint yet so I won't commit until that's done. Here's [the Twitter post](https://twitter.com/johnmmweb/status/1031760152532201472).
<br />

### R1D16 20180821
#### freeCodeCamp

**Today's Progress:**

**Thoughts/Notes:**

**Link to work:**

#### Bloc.io

**Today's Progress:**

**Thoughts/Notes:**

**Link to work:**
<br />
