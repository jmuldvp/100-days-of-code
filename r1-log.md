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
Nothing for today.

#### Bloc.io

**Today's Progress:**
Made more progress through this checkpoint.  Still not done because it is a longer checkpoint.

**Thoughts/Notes:**
- I hope this makes more sense tomorrow. Right now, the material is giving what seems like very basic information on the plan to implement the ActiveRecord framework replacement.

**Link to work:**
Checkpoint still isn't done.  No code pushed yet. See Twitter [post](https://twitter.com/johnmmweb/status/1032135103047032833).
<br />

### R1D17 20180822
#### freeCodeCamp

**Today's Progress:**
None.

#### Bloc.io

**Today's Progress:**
Still trying to figure out all this code I was given. It's supposed to be teaching me more about ActiveRecord.

**Thoughts/Notes:**
- There isn't a lot of explanation on the code I'm being given.  Trying to Google what things mean and understand it.

**Link to work:**
No code to push today. Here's [the Twitter post](https://twitter.com/johnmmweb/status/1032486713136799746).
<br />

### R1D18 20180823
#### freeCodeCamp

**Today's Progress:**
No progress tonight.

#### Bloc.io

**Today's Progress:**
Completed the checkpoint *Databases: Create an ORM*.  Started on the assignment. Read articles and watched videos on Ruby `super`, inheritance and even one on polymorphism.

**Thoughts/Notes:**
- lazy loading = It's not calculated until the first time it is needed.
- > Lazy loading contrasts with another pattern, which would calculate @schema when the model object is initialized. This pattern is called [eager loading](https://stackoverflow.com/questions/1299374/what-is-eager-loading/1299381#1299381).
- Learned about `super` and inheritance.

Questions for Rick:
1. Why would you write something that was going to return a schema instead of data?
2. Why would you use a heredoc.  Statement under picture of Terminator gif.
3. What does this mean?
> convert_keys takes an options hash and converts all the keys to string keys. This allows us to use either strings or symbols as hash keys. No matter which kind of keys are used, they're converted to string keys. This approach is similar to Rails'  HashWithIndifferentAccess.

4. Why is the heredoc structured like this...
```
connection.execute(<<-SQL)[0][0]
  SELECT COUNT(*) FROM #{table}
SQL
```
...but also like this...
```
connection.execute <<-SQL
  INSERT INTO #{table} (#{attributes.join ","})
  VALUES (#{vals.join ","});
SQL
```

**Link to work:**
The link to my work on [*address-bloc-orm*](https://github.com/jmuldvp/address-bloc-orm/tree/address-setup).
The linke to my work on [*bloc_record*](https://github.com/jmuldvp/bloc_record/tree/master).
<br />


### R1D19 20180824
#### freeCodeCamp

**Today's Progress:**
No freeCodeCamp progress today.

#### Bloc.io

**Today's Progress:**
Completed the *Databases: Create an ORM* checkpoint.

**Thoughts/Notes:**
- Learned the difference between `extend` and `include`.
> include: adds methods from the provided Module to the object

> extend: calls include on the singleton class of the object

..courtesy of this [page](https://aaronlasseigne.com/2012/01/17/explaining-include-and-extend/) among others like [this one](https://stackoverflow.com/questions/156362/what-is-the-difference-between-include-and-extend-in-ruby).

- Also learned the terms eager, lazy and over-eager loading [here](https://stackoverflow.com/questions/1299374/what-is-eager-loading/1299381#1299381).

**Link to work:**
Here's my *bloc-record* [repo](https://github.com/jmuldvp/bloc_record/tree/cp2-assign).
<br />

### R1D20 20180827
#### freeCodeCamp

**Today's Progress:**
None.

#### Bloc.io

**Today's Progress:**
- Almost got through the 3rd checkpoint of ORM but got stuck on some errors.

**Thoughts/Notes:**
- * is the splat operator. When used in the parameter section of a method like so..
```
def find(*ids)
end
```
.. it means it can take any number of arguments.

- Not sure if there are rules on when private methods should be used. Sent message to Rick.
- Studied about Ruby zip [here](http://www.rubyguides.com/2017/10/array-zip-method/) and [here](https://github.com/jmuldvp/address-bloc-orm/tree/cp3).

**Link to work:**
[Here](https://github.com/jmuldvp/bloc_record/tree/cp3) and [here](https://github.com/jmuldvp/address-bloc-orm/tree/cp3).
<br />


### R1D21 20180828
#### freeCodeCamp

**Today's Progress:**
Completed all of the FlexBox challenges.

**Thoughts/Notes:**
- `flex-wrap` does as it says..to wrap items when a space is too small.  The default setting/attribute is `nowrap`.
  - Options for this is `nowrap`, `wrap`, `wrap-reverse`.
- `flex-shrink` this allows an item to shrink if the flex container is too small. An example would be `flex-shrink: 3;` and `flex-shrink: 1;` where the one with 3 will shrink three times as fast as the one with 1.
- The opposite of `flex-shrink` is `flex-grow`. Also if the number/setting is bigger it grows that much faster.
- `flex-basis` specifies the initial size before CSS makes adjustments. If `auto` is used, it sizes items based on the content.
- Using the flex shorthand property can set several at once for `flex-grow`, `flex-shrink` and `flex-basis`.
>For example, flex: 1 0 10px; will set the item to flex-grow: 1;, flex-shrink: 0;, and flex-basis: 10px;.

- The `order` property will does like it says..order the items accordingly. Ex. `order: 1;` in one div or container and `order: 2;` in another.
- The `align-self` property allows you to adjust each items alignment individually instead of setting them all at once.
>This is useful since other common adjustment techniques using the CSS properties `float`, `clear`, and `vertical-align` do not work on flex items.

This property will override the `align-items` property.

**Link to work:**
No code to push. See [Twitter post](https://twitter.com/johnmmweb/status/1034651770029395970).

#### Bloc.io

**Today's Progress:**
Still stuck on a checkpoint because the instructions are all that clear.  I keep getting an error about a path when trying to run `bundle exec ruby db/seed.rb`

**Thoughts/Notes:**
- Frustration is all I can say about the instructions I was given in creating a ruby GEM. They aren't clear and I'm not getting the right help.

**Link to work:**
No code to push tonight to GitHub.
<br />


### R1D22 20180829
#### freeCodeCamp

**Today's Progress:**
Completed half of the CSS grid challenges.

**Thoughts/Notes:**
- Simply adding `disply: grid;` an HTML element into a grid container. The parent is referred to as the container and the children are call items.
- After setting up the _grid_, create columns like so.. `grid-template-columns: 100px 100px 100px`.
- To set the rows, one would use `grid-template-rows: 50px 50px;` as an example.
- Size units that could be used are as follows..
  - `fr` = Set the column/row to a fraction of the available space
  - `auto` = sets column/row content automatically
  - `%` = adjusts column/row to the percent width of it's container
- Using `grid-column-gap: 20px;` will space the columns.
- Same as above but for rows.. `grid-row-gap: 5px;`
- `grid-gap` is the same as using the column and row declarations. `grid-gap: 5px;` will affect rows and columns. `grid-gap: 5px 10px` will gap the rows 5px and columns 10px.
- `grid-column: 2 / 4;` will make a container take up the last 2 columns of a grid.
- `grid-row: 2 / 4;` does the same thing but for rows.
- `justify-self: center;` moves the content to the center. Other 2 options are `start` and `end`.
- Just like `justify-self` moves things horizontally, `align-self` does the same thing vertically.

**Link to work:**
No code to push. Here's [the Twitter post]().

#### Bloc.io

**Today's Progress:**
Completed the checkpoint material.  I had to change a bunch of `require`'s to `require_relative`'s and the code worked.

**Thoughts/Notes:**
- Really tough reading between the lines on assignment instructions on my school material.
  - The first assignment is to add some errors and data validation.  I thought I had to use ActiveRecord `validates` function.  Instead I figured that I should compare the data input to a regex for a phone number and an email address. Valid regex for phone and email..
  ```
  VALID_PHONE_REGEX = /\A(\+\d{1,2}\s)?\(?\d{3}\)?[\s.-]?\d{3}[\s.-]?\d{4}\z/
  VALID_EMAIL_REGEX = /\A[\w+\-.]+@[a-z\d\-]+(\.[a-z]+)*\.[a-z]+\z/i
  ```
  - I get the high level concept of `method_missing` but still haven't been able to find a good example on how to use it.
    - Found a good example [here](https://technicalpickles.com/posts/using-method_missing-and-respond_to-to-create-dynamic-methods).  Just having a hard time trying to figure out how to make it work with my assignment. Here's the code I'm going to try and implement in my assignment..
    ```Ruby
    class LegislatorDynamicFinderMatch
      attr_accessor :attribute
      def initialize(method_sym)
        if method_sym.to_s =~ /^find_by_(.*)$/
          @attribute = $1.to_sym
        end
      end

      def match?
        @attribute != nil
      end
    end

    class Legislator    
      def self.method_missing(method_sym, *arguments, &block)
        match = LegislatorDynamicFinderMatch.new(method_sym)
        if match.match?
          define_dynamic_finder(method_sym, match.attribute)
          send(method_sym, arguments.first)
        else
          super
        end
      end

      protected

      def self.define_dynamic_finder(finder, attribute)
        class_eval <<-RUBY
          def self.#{finder}(#{attribute})        # def self.find_by_first_name(first_name)
            find(:#{attribute} => #{attribute})   #   find(:first_name => first_name)
          end                                     # end
        RUBY
      end
    end
    ```
    - Not sure why I keep seeing a lot of code turning things into symbols. Gonna have to read up on why symbols are so good to use.

**Link to work:**
My [link to the checkpoint code](https://github.com/jmuldvp/address-bloc-orm/tree/cp3).
<br />


### R1D23 20180830
#### freeCodeCamp

**Today's Progress:**
No progress today.

#### Bloc.io

**Today's Progress:**
Completed step 2 on the assignment for `method_missing`.

**Thoughts/Notes:**
- Found out using `class_eval` is slow. Rick showed me how to accomplish this in 2 lines.
- Stuck on step 3 of the assignment now.  I'm not sure how to implement `find_each` with `batch_size` support all in the same method where both of these are supposed to work..

```Ruby
Contact.find_each do |contact|
  contact.check_if_naughty_or_nice
end
```
..or..
```Ruby
Contact.find_each(start: 2000, batch_size: 2000) do |contact|
  contact.check_if_naughty_or_nice
end
```
..are supposed to work with one method.

**Link to work:**
No code to push tonight. [Here is the Twitter post](https://twitter.com/johnmmweb/status/1035380245484859392).
<br />

### R1D24 20180904
#### freeCodeCamp

**Today's Progress:**
None tonight.

#### Bloc.io

**Today's Progress:**
Progress was very slow going. Trying to implement `find_each` with support of `batch_size` and `find_in_batches`.  The documentation really frustrates me because it isn't detailed and I feel the documentation should be spot on for a school that I paid a lot of money to.  I know documentation isn't going to exist or be good in the outside world but I feel that if someone is going to take that much money from me for me to learn, their documentation should be flawless so I don't have to try and read between the lines.  I almost feel like I paid a bunch of money for someone to tell me to use Google whenever I get stuck.

**Thoughts/Notes:**
Plan of attack so far..
- Going to create separate methods for `find_each` and `find_in_batches`. It doesn't make sense that I would put `find_in_batches` within the `find_each` method because I don't know how I'd call it given the examples I was given in the assignment.

**Link to work:**
No code to push tonight. Here's [my Twitter post](https://twitter.com/johnmmweb/status/1037195270554116096).
<br />


### R1D25 20180905
#### freeCodeCamp

**Today's Progress:**
None.

#### SoloLearn
Acquired 290 XP on SoloLearn.

#### Bloc.io

**Today's Progress:**
Still no progress on this. I can't get a straight answer to my questions from the technical coaches. Meeting with my instructor tomorrow night so hopefully I can get past it then.  I did perform Google searches but nothing helped.

**Thoughts/Notes:**
- Note to self: don't ever try and explain programming like this Bloc material does. People won't understand it.

**Link to work:**
No new code. Here's [my Twitter post](https://twitter.com/johnmmweb/status/1037585314871529472).
<br />

### R1D26 20180906
#### SoloLearn
I increased my XP to 337 by working on HTML, SQL and Ruby exercises.

#### freeCodeCamp

**Today's Progress:**
Completed the CSS Grid challenges.

**Thoughts/Notes:**
- `justify-items: center;` will align all items in the container at once vs the way that could be used to align items individually.
- `align-items` property on a grid container will set the vertical alignment.
- `grid-template-areas:` is used for grouping cells. Here's an example..
```
grid-template-areas:
  "header header header"
  "advert content content"
  "footer footer footer";
```
If you use a period . it gives the indication that the space is blank.
- `grid-area` will place the cell in a named grid area like `header` or `footer`.
>- If your grid doesn't have an areas template to reference, you can create an area on the fly for an item to be placed. `item1 { grid-area: 1/1/2/4; }`  Here is the cheat sheet for the numbers mentioned..
>grid-area: horizontal line to start at / vertical line to start at / horizontal line to end at / vertical line to end at;

- If you want to setup a grid with many rows or columns, instead of typing the code over and over again, you could use `repeat`. This creates 100 rows 50px tall... `grid-template-rows: repeat(100, 50px);` This `grid-template-columns: 1fr 1fr 1fr;` translates to this `grid-template-columns: repeat(3, 1fr);`
- `minmax` is used to limit the size of items. This example `grid-template-columns: 100px minmax(50px, 200px);` sets the size of the columns 100px wide. It also limits the size to 50px on the small end and 200px on the large end.
- The repeat function comes with an option called auto-fill.
>When the container changes size, this setup keeps inserting 60px columns and stretching them until it can insert another one.
Note
If your container can't fit all your items on one row, it will move them down to a new one.

> - auto-fit works almost identically to auto-fill. The only difference is that when the container's size exceeds the size of all the items combined, auto-fill keeps inserting empty rows or columns and pushes your items to the side, while auto-fit collapses those empty rows or columns and stretches your items to fit the size of the container.

- Making a layout responsive by using `@media`...
```
@media (min-width: 400px){
  .container{
    /* change the code below this line */

    grid-template-areas:
      "header header"
      "advert content"
      "footer footer";

  /* change the code above this line */
  }
}
```
**Link to work:**
N/A Here's [the Twitter post](https://twitter.com/johnmmweb/status/1037936489831661569).

#### Bloc.io

**Today's Progress:**
Met with my mentor tonight. I may have the `find_each` and `find_in_batches` assignment solved.  I'll find out for sure once it's graded.

**Thoughts/Notes:**
- Rick gave more information on using `yield`. He even stated that the documentation I was given to do the assignment was confusing because it was even confusing for him.

**Link to work:**
<br />

### R1D27 20180907
#### freeCodeCamp

**Today's Progress:**
Started on the tribute page on codepen.

**Thoughts/Notes:**
- The instructions are pretty detailed which is good. I'm hoping I can spend a little more time on it than just the basics.

**Link to work:**
Here's [what I have so far](https://codepen.io/jmuldvp/pen/vJpgEO).
Here's [the Twitter post](https://twitter.com/johnmmweb/status/1038296998850396160).

#### SoloLearn

**Today's Progress:**
Only worked on a little SQL. Up to 342 XP.

#### Bloc.io

**Today's Progress:**
I think I finished checkpoint 3 assignment...after 2 weeks of struggling.

**Thoughts/Notes:**
- I'm going to have to go back and study this method a little more...
```ruby
def rows_to_array(rows)
  rows.map { |row| new(Hash[columns.zip(row)])}
end
```
I'm still not sure I can describe what `zip` does.

**Link to work:**
Here's my [branch](https://github.com/jmuldvp/bloc_record/tree/cp3-assign).
<br />

### R1D28 20180910
#### freeCodeCamp

**Today's Progress:**
None today.

#### SoloLearn

**Today's Progress:**
None today.

#### Bloc.io

**Today's Progress:**
Almost completed checkpoint 12 of the SQL section. I completed over half of the assignment.

**Thoughts/Notes:**
- Subqueries in the `FROM` clause are *inline views*.
>- Subqueries in the `WHERE` clause can be used with either a row constructor or an expression.

- Row constructor - an expression that builds a row using values for it's member fields.
>- When using `IN`, `NOT IN`, `ANY`, `SOME`, or `ALL`, the subquery must return data in only 1 column.

>- `EXISTS`: If the subquery returns at least one row, the `EXISTS` returns `true`; otherwise, it returns `false`.

>- `NOT EXISTS`: If the subquery does not return at least one row, the `EXISTS` returns  `true`; otherwise, it returns `false`.

>- `IN`: The result of IN is `true` if any matching subquery row is found; otherwise, the result is `false` if no matching row is found. If the subquery returns no rows, the result is also `false`; however, if the left-hand side evalutes to NULL, the result will be  `NULL`.

>- `NOT IN`: When using `NOT IN`, the subquery must return exactly 0 matching rows. Each department is allocated a certain budget annually for salary.

>- `ANY` & `SOME`: `ANY` and `SOME` are equivalent.

They are also pretty self explanatory
- `ALL`: For `ALL` to return `true` *either* every result returned by the subquery must match the given condition or the subquery must return no rows.
- Subqueries can be more readable than `join`'s and they can eliminate duplication.

**Link to work:**
The assignment was all SQL queries. No code to push.  Here's [the Twitter post](https://twitter.com/johnmmweb/status/1039403539917729792).


### R1D29 20180911
#### freeCodeCamp

**Today's Progress:**
I'm hoping to put some more time into this tomorrow. None today.

#### SoloLearn

**Today's Progress:**
- Knocked out some more of the SQL fundamentals section and a few Ruby exercises.

#### Bloc.io

**Today's Progress:**
Completed checkpoint 12. Got a 4/6 on the quiz. There were questions in that quiz covering material that wasn't in the checkpoint.

**Thoughts/Notes:**
- It was good to learn some more Postgres syntax.

**Link to work:**
Here [is my push to GitHub](https://github.com/jmuldvp/bloc-rdbf/blob/master/cp12/CP12-answers.md).

### R1D30 20180912
#### freeCodeCamp

**Today's Progress:**
None.

#### SoloLearn

**Today's Progress:**
Covered more HTML. Up to 365XP.

#### Bloc.io

**Today's Progress:**
Completed the checkpoint material.

**Thoughts/Notes:**
- Very good [reference](https://stackoverflow.com/questions/2307283/what-does-olog-n-mean-exactly) for determining complexity.
- Started the assignment.

**Link to work:**

### R1D31 20180913
#### freeCodeCamp

**Today's Progress:**
I'm probably going to put this on the back burner for awhile...maybe.

#### SoloLearn

**Today's Progress:**
Reviewed HTML colors and the `frame` tag...which is not supported in HTML5.  Seems like CSS-Grid and FlexBox covers that now.

#### Bloc.io

**Today's Progress:**
Completed the assignment on the 4th checkpoint on algorithms and complexity. Started on the main part of checkpoint 5.

**Thoughts/Notes:**
- Under the heading of Linear Time Complexity: O(n), here's some code that I typed in..

```ruby
# #1
def linear_search(collection, value)
  # #2
  for i in collection
    return i if i == value
  end
end
```

>At #1, we see the method definition, this line of code does not affect the complexity.

>At #2, we iterate over `collection`. This is the meat of linear search. Let's think about this loop in the context of our worst case scenario: in the worst case the item we're searching for, `value` will be at the `collection.length-1` index. So, our algorithm's worst case performance is O(`collection.length - 1`), but we really don't care about the -1 so we can drop it. Thus, our algorithm is O(`collection.length`), but `collection.length` is really just another way of expressing n, an arbitrary integer. The complexity of linear search is therefore *O(n)*.

- Under the heading of Logarithmic Time Complexity: O(log n), I typed in some given code for a binary search.
- Used a `while` loop to divide and conquer for a binary search.

**Link to work:**
Here's [my work for checkpoint 4](https://github.com/jmuldvp/bloc-algorithms-complexity/blob/master/cp4/intro_complexity_answers.md).

### R1D32 20180918
#### freeCodeCamp

**Today's Progress:**
None.

#### SoloLearn

**Today's Progress:**
None.

#### Bloc.io

**Today's Progress:**
Completed checkpoint material and now I'm stuck on the assignment. I'm trying to determine the Big-O notation on a numbers algorithm.

**Thoughts/Notes:**
- Trying to figure out how many iterations an algorithm goes through before completion.

**Link to work:**
No code to push tonight.

### R1D33 20180919
#### freeCodeCamp

**Today's Progress:**
None.

#### SoloLearn

**Today's Progress:**
None.

#### Bloc.io

**Today's Progress:**
Completed a checkpoint assignment.

**Link to work:**
Here's the [link](https://github.com/jmuldvp/bloc-algorithms-complexity/tree/cp5-assign).

### R1D34 20180920
#### freeCodeCamp

**Today's Progress:**
None.

#### SoloLearn

**Today's Progress:**
None.

#### Bloc.io

**Today's Progress:**
Revisited checkpoing 4 and completed it. I misunderstood the instruction.

**Link to work:**
[Here is my work](https://github.com/jmuldvp/bloc-algorithms-complexity/tree/cp4-assign/cp4).

### R1D35 20180926
#### freeCodeCamp

**Today's Progress:**
None today.

#### SoloLearn

**Today's Progress:**
None today.

#### Bloc.io

**Today's Progress:**
I may have finished another assignment.  I have to go back through and review a few spots that I'm still a bit shady on.

**Thoughts/Notes:**
- Using hashing functions aren't as easy as I thought it was going to be.

**Link to work:**
I have no pushed the final code for this assignment.  I'll do that tomorrow.

### R1D36 20181001
#### freeCodeCamp

**Today's Progress:**
None.  Been concentrating on my material for Bloc.io

#### SoloLearn

**Today's Progress:**
Made progress in HTML, SQL, Ruby and CSS.  Learned that I can use a case statement like this...
```ruby
case 1,2,3
```
..when I want to check for those specific numbers. As far as ranges are concerned, when there are 2 dots, it includes the first and last number.  When there are 3 dots, the first number the number before the last are used.  Also, I knew about `break`, I forgot about `next` and I didn't know about `redo` inside loops.

I knew all the topics discussed in the SQL section.

#### Bloc.io

**Today's Progress:**
Watched video of my meeting last week with mentor.  I think I'm finished but don't feel comfortable moving on just yet.

**Thoughts/Notes:**
- Hashes make a little more sense but still not entirely clear. Going to look for video's and more documentation.

**Link to work:**
Pushed code [here](https://github.com/jmuldvp/bloc-data-structures).

### R1D37 20181002
#### freeCodeCamp

**Today's Progress:**
None.

#### SoloLearn

**Today's Progress:**
None.

#### Bloc.io

**Today's Progress:**
Learned about a few efficient algorithm changes that could be made in loops.

**Thoughts/Notes:**
- Learned more about efficiency and the thoughts of even the simplest changes can save many CPU cycles if the logic is implemented into an application that runs it all day.

**Link to work:**
None today. Looked at and pondered about algorithms and how to make things go faster or cleaner.


### R1D38 20181003
#### freeCodeCamp

**Today's Progress:**
None.

#### SoloLearn

**Today's Progress:**
- 7 new content models in HTML5
  - Metadata Content that sets up the presentation or behavior of the rest of the content. `<base>, <link>, <meta>, <noscript>, <script>, <style>, <title>`
  - Embedded This imports other resources into the doc.. `<audio>, <video>, <canvas>, <iframe>, <img>, <math>, <object>, <svg>`
  - Interactive Meant for user interaction. `<a>, <audio>, <video>, <button>, <details>, <embed>, <iframe>, <img>, <input>, <label>, <object>, <select>, <textarea>`
  - Heading Header section.  `<h1> thru <h6> and then <hgroup>`
  - Phrasing Has a number of inline elements in common with HTML4 such as `<img>, <span>, <strong>, <label>, <br />, <small>, <sub>` and more.
  - Flow This contains the majority of HTML5 elements that would be in the normal flow of the document.
  - Sectioning Defines scope of headings, content, navigation and footers. `<article>, <aside>, <nav>, <section>`
- Can remove items from one array using another array like so...

```ruby
a = [1, 2, 3, 4, 5]
b = [2, 4, 5, 6]

res = a - b
print res #[1, 3]
```
- Can also duplicate array data.. *For example: [1, 2, 3] * 3 results in [1, 2, 3, 1, 2, 3, 1, 2, 3]*
- Can also compare 2 arrays and print similar values...
```ruby
a = [2, 3, 7, 8]
b = [2, 7, 9]

print a & b # [2, 7]
```
- Using the | operator, one could do this to combine arrays like a union all statement in SQL..
```ruby
a = [2, 3, 7, 8]
b = [2, 7, 9]

print a | b # [2, 3, 7, 8, 9]
```
- Using `.reverse` will reverse the values of an array. Using the `!` symbol will permanently change the value of the variable.

#### Bloc.io

**Today's Progress:**
Almost finished with another checkpoint.  Hopefully I'll be able to finish it up tomorrow.

**Thoughts/Notes:**
- Code optimization advice...
> Code can be optimized by pruning unused statements, assignments, or adding shortcuts such as ending a loop early if possible. Although pruning bad code _will improve performance_, it won't necessarily _improve complexity_.

- I almost feel like using `.flatten` in my second assignment is cheating but I'm glad I found out about it.

**Link to work:**
I did not push my final code tonight.

### R1D39 20181004
#### freeCodeCamp

**Today's Progress:**
None today.

#### SoloLearn

**Today's Progress:**
- SQL data types..
  - Numberic = `int`, `float`, `double`
  - Date and Time = `date`, `datetime`, `timestamp`, `time`
  - String type = `char`, `varchar`, `blob`, `text`
- UNIQUE = Does not allow to insert a duplicate value in a column. The UNIQUE constraint maintains the uniqueness of a column in a table. More than one UNIQUE column can be used in a table.
- CHECK = Determines whether the value is valid or not from a logical expression.
```sql
UserID int NOT NULL AUTO_INCREMENT,
PRIMARY KEY (UserID)
```

```sql
CREATE TABLE Users (
id int NOT NULL AUTO_INCREMENT,
username varchar(40) NOT NULL,
password varchar(10) NOT NULL,
PRIMARY KEY(id)
);
```
- `Alter Table` command is used to alter a tables columns by adding, removing or changing data types.
```sql
ALTER TABLE People ADD DateOfBirth date;
```
You can also use `DROP` instead of `ADD`. One could also change the name of a column with this command...
```sql
ALTER TABLE People CHANGE FirstName name varchar(100);
```

- To rename a table... `RENAME TABLE People TO Users;`
- To create a view...
```sql
CREATE VIEW view_name AS
SELECT column_name(s)
FROM table_name
WHERE condition;
```
- Completed SQL Fundamentals course.

#### Bloc.io

**Today's Progress:**
Completed checkpoint 6. Not sure if I did number 3 of the assignment correctly since the instructions weren't all that clear.

**Thoughts/Notes:**
- To optimize code, remove unnecessary loops.
- `do each` is more expensive than using an `if` to remove unwanted/invalid input.
- If I can remove any unnecessary comparison(s), that would be an optimization.

**Link to work:**
Pushed to Github.

### R1D40 20181009
#### freeCodeCamp

**Today's Progress:**
None.

#### SoloLearn

**Today's Progress:**
Completed the HTML course and obtained certificate. Worked on the Ruby and JavaScript courses.  I did a lot of this today along with looking at JavaScript blogs to prep for a test I took.

#### Bloc.io

**Today's Progress:**
Completed reading through a checkpoint on data structures learning more about hashes, collisions etc. Still need to take some notes on Linear and Quadratic probing along with Double Hashing. Then need to look more into Cuckoo Hashing.

**Thoughts/Notes:**
- Separate Chaining = this helps resolve collisions. This process tacks on colliding entries to the same location in the array and refers to that same location as a bucket. In order to tack on an entry to another using a linked list.
- Load Factor = This is an actual formula.  You take the number of entries and divide by the number of buckets which gives you a decimal number. A high load factor > .7 usually means slower performance.
- Open Addressing = When a collision occurs, this uses one of three approaches to resolve it. If it can't find an empty location, it increases the size of the hash.
  - Linear Probing = This looks for the next available bucket one at a time until it finds one.
  - Quadratic Probing
  - Double hashing

**Link to work:**
No code to push tonight. There was no code to try out in the checkpoint. Spent most of my night reading over JavaScript material to prep for a test I took.


### R1D41 20181010
#### freeCodeCamp

**Today's Progress:**
None.

#### SoloLearn

**Today's Progress:**
Made more progression on the Ruby track.

#### Bloc.io

**Today's Progress:**
Reread some of the checkpoint material trying to make the concepts sink deeper.

**Thoughts/Notes:**
None.

**Link to work:**
No code to push again today.

### R1D42 20181011
#### freeCodeCamp

**Today's Progress:**
None.

#### SoloLearn

**Today's Progress:**
Made more progress in Ruby.  Learned more about Accessor Methods and Class Methods and variables. I also learned how I can use `to_s` to modify a `puts` statement/line.

#### Bloc.io

**Today's Progress:**
Re-read some of the checkpoint material again and started on the assignment.

**Link to work:**
No code pushed.


### R1D43 20181015
#### freeCodeCamp

**Today's Progress:**
None.

#### SoloLearn

**Today's Progress:**
Some of the Ruby exercises.

#### Bloc.io

**Today's Progress:**
Got 2 tests to pass on the open_addressing part of the assignment.
c

### R1D44 20181023
#### freeCodeCamp

**Today's Progress:**
None

#### SoloLearn

**Today's Progress:**
None

#### Bloc.io

**Today's Progress:**
Completed an open addressing hash exercise and started on the separate chaining exercise.

**Thoughts/Notes:**
I had to put together a nested hash of sorts as a coding exercise.

**Link to work:**
Even though I didn't complete the exercise, I pushed what I had as a backup.


### R1D45 20181024
#### freeCodeCamp

**Today's Progress:**
None. I'm coming back to this at some point.

#### SoloLearn

**Today's Progress:**
None.

#### Bloc.io

**Today's Progress:**
Completed the linked_list.rb file for the separate_chaining exercise.



### R1D46 20181029
#### freeCodeCamp

**Today's Progress:**
None.

#### SoloLearn

**Today's Progress:**
Made more progress with the Ruby section.

#### Bloc.io

**Today's Progress:**
Completed the second hashing assignment (Checkpoint 5) where I learned more about hashing functions. Started on the last checkpoint for algorithms.

**Thoughts/Notes:**
> - Algorithms that have Big-O of polynomial time or less are referred to as tractable.
> - An algorithm is said to be of polynomial time (or tractable) if its running time is upper bounded by a polynomial expression in the size of the input for the algorithm. - [Wikipedia](https://en.wikipedia.org/w/index.php?title=Cobham%27s_thesis&redirect=no)

- Famous polynomial time algorithms...
  - Breadth First search
  - Depth First Search
  - Cocktail Sort
  - Gnome Sort
  - Comb Sort
  - Dijkstra's Algorithm
> - In computer science, a hard problem is defined as a problem for which there is no known solution that has a Big-O with less than or equal to polynomial time. These sets of problems are called intractable or non-polynomial time problems.

- Intractable problems are referred to as NP Hard.

**Link to work:**
Here's my [submission](https://github.com/jmuldvp/bloc-data-structures/tree/master/05-hashes-part-2)


### R1D47 20181030
#### freeCodeCamp

**Today's Progress:**
None.

#### SoloLearn

**Today's Progress:**
- Modules should start with a capital letter.
- An example of a "mix"...
```ruby
module Flyable
  def fly
    puts "I'm flying!"
  end
end

class Vehicle
end

class Car < Vehicle
end

class Jet < Vehicle
  include Flyable
end

class Plane < Vehicle
  include Flyable
end

ob = Jet.new
ob.fly
```

- Classes can only inherit from one other class.  But one class can inherit from multiple modules like so...
```ruby
class Human
  include Walkable
  include Speakable
  include Runnable
end
```

- If it's an "is-a" relationship, choose class inheritance. If it's a "has-a" relationship, choose modules. Example: a plane "is a" vehicle; a plane "has an" ability to fly.
- You cannot instantiate modules (i.e., an object cannot be created from a module).
Modules are used only for grouping common methods together.
Classes are about objects; modules are about methods.
- `Comparable` is a built-in mixin.  It is used to add the comparison operators to a class. `<, <=, ==, >=, >`
- Example of namespacing...
```ruby
module Mammal
  class Dog
    def speak
      puts "Woof!"
    end
  end
  class Cat
    def speak
      puts "Meow"
    end
  end
end

a = Mammal::Dog.new
b = Mammal::Cat.new

a.speak  # "Woof"
b.speak  # "Meow"
```

#### Bloc.io

**Today's Progress:**
This task will probably take multiple nights. I'm trying to learn how to put together an implementation of the traveling salesman in Ruby.

**Thoughts/Notes:**
- Notes on implementation 1:
  - Created `City` class with `name` and `visited` variables.
  - Instantiated instances of 5 cities and also an array with those 5 instantiations.
  - Created `Trip` class with 3 variables for the first city, second city and distance.
  - Created 20 trips listing the different distances between each city... `trip1` thru `trip20` and then put each trip instance in an array.
  - Created a traveling salesman method which takes the cities and trips array and also the first city to start with.

**Link to work:**


### R1D48 20181031
#### freeCodeCamp

**Today's Progress:**
None.

#### SoloLearn

**Today's Progress:**
- Struct = a built-in Ruby class and makes it shorter to define simple classes, accessors, and their initialize methods. Here is an example...
```ruby
Point = Struct.new(:x, :y)

origin = Point.new(0, 0)
dest = Point.new(15, 42)

puts dest.y  # 42
```

- OpenStruct (or OStruct) acts very similarly to Struct, except that it doesn't have a defined list of attributes. Here's an example...
```ruby
require "ostruct"

person = OpenStruct.new
person.name = "John"
person.age = 42
person.salary = 250

puts person.name  # John
```

- OStruct isn't as fast as Struct, but it is more flexible.
- Can also initialize an OStruct using a hash like so...
```ruby
require "ostruct"

person = OpenStruct.new(name:"John", age:42, salary:250)

puts person.name  # John
```

- Struct and OStruct provide a simple way to create data structures that have the behavior of a class.
- Examples of built-in classes are `Array`, `String` and `Struct`. Another built-in class is the `Math` class. Here are some examples...
```ruby
# square root
puts Math.sqrt(9) # 3

# pi constant
puts Math::PI

# trigonometry (sin, cos, tan)
puts Math::cos(0) # 1
```

- Another built-in class is `Time`.  Here are some examples...
```ruby
# current time
t = Time.now
puts t

# year, month, day
puts t.year
puts t.month
puts t.day

# custom date
t = Time.new(1988, 6, 10)

# day of week: 0 is Sunday
puts t.wday

# day of year
puts t.yday
```

- Procs give the ability to take a block of code, store it in a variable and run that block whenever necessary. Example...
```ruby
greet = Proc.new do |x|
  puts "Welcome #{x}"
end
```

- This is how you'd use the above code...
```ruby
greet.call "David"
greet.call "Amy"

# Outputs
# "Welcome David"
# "Welcome Amy"
```

- Procs can be passed into methods like so...
```ruby
greet = Proc.new do |x|
  puts "Welcome #{x}"
end

goodbye = Proc.new do |x|
  puts "Goodbye #{x}"
end

def say(arr, proc)
  arr.each { |x| proc.call x}
end

people = ["David", "Amy", "John"]
say(people, greet)
say(people, goodbye)
```

- We can pass to our methods as many procs as we want.
- Example of a proc to count the execution time of a block of code.
```ruby
def calc(proc)
  start = Time.now
  proc.call
  dur = Time.now - start
end

someProc = Proc.new do
  num = 0
  1000000.times do
    num = num + 1
  end
end

puts calc(someProc)
```

- A lambda is an instance of a Proc class. To create one... `talk = lambda{puts "Hi"}` or `talk = ->() {puts "Hi"}`.
- Just like with procs this is how a lambda is called.. `talk.call`.
- In other programming languages, a lambda is commonly referred to as an anonymous function.
- Lambda's check the number of arguments and procs do not. Take this code that works...
```ruby
talk = lambda { |x| puts "Hello #{x}" }
talk_proc = Proc.new { |x| puts "Hello #{x}" }

talk.call "David"
# outputs "Hello David"

talk_proc.call "Amy"
# outputs "Hello Amy"
```

- This code error's out because of the argument...
```ruby
talk_proc.call
# ouputs Hello

talk.call
# outputs "Error: wrong number of arguments (given 0, expected 1)"
```

> - A second difference between a lambda and a Proc is how the return statement is handled.
When a lambda encounters a return statement it returns execution to the enclosing method.
However, when a Proc encounters a return statement it jumps out of itself, as well as the enclosing method.

-

#### Bloc.io

**Today's Progress:**
More studying of the traveling salesman implementations.

**Thoughts/Notes:**
- Forgot that the double less than `<<` means that a value is being added to the end of an array. Can also for a heredoc like so...
```ruby
up_here_doc = <<_stuff_
This is a test of the emergency broadcast system. Had this been an actual emergency..
...
_stuff_
```

- Implemented a Proc and a Struct instead of creating a class and method.

**Link to work:**
Here's my [work](https://github.com/jmuldvp/bloc-algorithms-complexity/tree/master/cp7).


### R1D49 20181101
#### freeCodeCamp

**Today's Progress:**
None.

#### SoloLearn

**Today's Progress:**
- Create a new file `file = File.new("test.txt", "w+")`
- To close the file `file.close`.
>- It is necessary to close open files so they no longer continue to occupy space in memory.

- These are the modes for working with files...
```
r read-only, starts at beginning of file (default mode).
r+ read-write, starts at beginning of file.
w write-only, truncates existing file to zero length or creates a new file for writing.
w+ read-write, truncates existing file to zero length overwriting existing data or creates a new file for reading and writing.
a write-only, appends to end of file if file exists, otherwise creates a new file for writing.
a+ read-write, appends or reads from end of file if file exists, otherwise creates a new file for reading and writing.
```

- To open an existing file... `file = File.open("filename", "w+")`
- One way that a file can be created, written to and then closed...
```ruby
file = File.new("test.txt", "w+")
file.puts("some text")
file.close
```

- One could use a code block to do the same thing...
```ruby
File.open("file.txt", "w+") {
  |file| file.puts("some text")
}
```

- Here's how to read the entire contents of a file...
```ruby
f = File.new("test.txt", "w+")
f.puts("a line of text")
f.puts("another line of text")
f.close

puts File.read("test.txt")
```

- Here's how a file can be read line by line...
```ruby
File.open("test.txt", "a+") {
  |file| file.puts("a line of text")
  file.puts("another line of text")
}

File.readlines("test.txt").each {
  |line| puts " --- #{line}"
}
```

- The readlines method reads the entire file based on individual lines and returns those lines in an array.
- Here is how a file can be deleted `File.delete("test.txt")`. This is a permanent deletion.
- This checks to see if a file exists in order to prevent an error... `File.open("test.txt") if File.file?("text.txt")`.
- To grab some file information...
```ruby
# create a file
f = File.new("test.txt", "w+")
f.puts("some file content")

puts f.size # 19

f.close

puts File.zero?("test.txt") # false
```

- Can check to see if the file is writable, readable or executable..
```ruby
f = File.new("test.txt", "w+")
f.puts("some content")
f.close

puts File.readable?("test.txt") # true
puts File.writable?("test.txt")   # true
puts File.executable?("test.txt") # false
```

- Completed the Ruby section.

#### Bloc.io

**Today's Progress:**
Completed checkpoint 3 of ORM. This is really confusing creating my own ActiveRecord replacement but it does make sense here and there.  I could easily write the sql needed but to try and create an ActiveRecord replacement isn't easy.

**Thoughts/Notes:**
- Trying to find and study implementations of the exercise to allow these kinds of calls using strings or symbols...
```ruby
Entry.order(:name, phone_number: :desc)
# or
Entry.order(name: :asc, phone_number: :desc)
# or
Entry.order("name ASC, phone_number DESC")
# or
Entry.order("name ASC", "phone_number DESC")
```

**Link to work:**
None.


### R1D50 20181105
#### freeCodeCamp

**Today's Progress:**
None.

#### SoloLearn

**Today's Progress:**
None.

#### Bloc.io

**Today's Progress:**
Finished the SQL challenge and tried to implement a sort option in the Bloc_Record project.

**Thoughts/Notes:**
Stuck on trying to implement the sort action within Address-Bloc.

**Link to work:**
None.

### R1D51 20181106
#### freeCodeCamp

**Today's Progress:**
None.

#### SoloLearn

**Today's Progress:**
Working on JavaScript now. Finished some familiar concepts of if/else and also the `switch` statement.

#### Bloc.io

**Today's Progress:**
Completed ORM arch checkpoint on `where`, `order` and `joins`. Started on the data structure checkpoint on binary trees. Now I'm working on the assignment where I have to implement `insert`, `find`, `delete` and `printf`.

**Thoughts/Notes:**
- Tree's consist of *Nodes*.
- Tree's grow from the top down.
- A node may only have at most 2 child nodes.
- Nodes without children are called leaf nodes.
- A Heap is also a tree.
- Binary Heap...
>A binary heap is a complete binary tree; that is, all levels of the tree, except possibly the last one (deepest) are fully filled, and, if the last level of the tree is not complete, the nodes of that level are filled from left to right.

- Here's the logic for inserting into a Binary Heap...
```
1. Insert a new node at the end of Heap.
2. Compare the value of the new child node with its parent.
3. If the value of parent node is less than child, then swap the parent node with the child node.
4. Repeat step 2 and 3 until the Heap property holds.
```

- Depth-First Search (DFS):
>DFS is the process of traveling down a single branch in search of the desired element. If you find it, hurray, but if not, you travel upwards and repeat the process with unvisited Nodes.

- Breadth-First Search (BFS):
>search an entire row of Nodes before we proceed to the next.

**Link to work:**
None.

### R1D52 20181114
#### freeCodeCamp

**Today's Progress:**
None.

#### SoloLearn

**Today's Progress:**
None.  I did work on the JavaScript section a few days ago but didn't log it until now.

#### Bloc.io

**Today's Progress:**
Trying to read through and to understand the assignment on min heap.


### R1D53 20181115
#### freeCodeCamp

**Today's Progress:**
None.

#### SoloLearn

**Today's Progress:**
None.

#### Bloc.io

**Today's Progress:**
Read more about how to put a min heap together with `insert`, `delete`, `find` and `print` methods.

**Thoughts/Notes:**
- Read a little about `public`, `private` and `protected` access within Ruby.

**Link to work:**


### R1D54 20181126
#### freeCodeCamp

**Today's Progress:**
None.

#### SoloLearn

**Today's Progress:**
Covered JS functions.
- Always remember to end the statement with a semicolon after calling the function.
- You can also call a function using this syntax: myFunction.call().

In regards to function parameters..
- If a function is called with missing arguments (fewer than declared), the missing values are set to undefined, which indicates that a variable has not been assigned a value.
- If you do not return anything from a function, it will return undefined.
- The document.write command outputs the value returned by the function, which is the sum of the two parameters.

*Alert box*
- An alert box is used when you want to ensure that information gets through to the user.
- When an alert box pops up, the user must click OK to proceed.
- To display line breaks within a popup box, use a backslash followed by the character n.

*Prompt Box*
- A prompt box is often used to have the user input a value before entering a page.
- When a prompt box pops up, the user will have to click either OK or Cancel to proceed after entering the input value.
- If the user clicks OK, the box returns the input value. If the user clicks Cancel, the box returns null.
- The prompt() method takes two parameters.
- The first is the label, which you want to display in the text box.
- The second is a default string to display in the text box (optional).

*Confirm Box*
- A confirm box is often used to have the user verify or accept something.
- When a confirm box pops up, the user must click either OK or Cancel to proceed.
- If the user clicks OK, the box returns true. If the user clicks Cancel, the box returns false.
```JavaScript
var result = confirm("Do you really want to leave this page?");
if (result == true) {
  alert("Thanks for visiting");
}
else {
  alert("Thanks for staying with us");
}
```

#### Bloc.io

**Today's Progress:**
None.


### R1D55 20181127
#### freeCodeCamp

**Today's Progress:**
None.

#### SoloLearn

**Today's Progress:**
*Objects*
- JavaScript objects are containers for named values.
- You can access object properties in two ways.
  - `objectName.propertyName`
  - `objectName['propertyName']`
- JavaScript's built-in length property is used to count the number of characters in a property or string.
```JavaScript
var course = {name: "JS", lessons: 41};
document.write(course.name.length);
//Outputs 2
```

- An object method is a property that contains a function definition.
- As you already know, document.write() outputs data. The write() function is actually a method of the document object.
- Methods are functions that are stored as object properties.

#### Bloc.io

**Today's Progress:**
None.

### R1D56 20181203
#### freeCodeCamp

**Today's Progress:**
None.

#### SoloLearn

**Today's Progress:**
Object constructor example:
```JavaScript
function person(name, age, color) {
  this.name = name;
  this.age = age;
  this.favColor = color;
}
```

- The this keyword refers to the current object. Note that this is not a variable. It is a keyword, and its value cannot be changed.
- Once you have an object constructor, you can use the new keyword to create new objects of the same type. Here's an example...
```JavaScript
var p1 = new person("John", 42, "green");
var p2 = new person("Amy", 21, "red");

document.write(p1.age); // Outputs 42
document.write(p2.name); // Outputs "Amy"
```

- Use the object literal or initializer syntax to create single objects like so...
```JavaScript
var John = {name: "John", age: 25};
var James = {name: "James", age: 21};
```

- Methods are functions that are stored as object properties.
```JavaScript
function person(name, age) {
  this.name = name;  
  this.age = age;
  this.changeName = function (name) {
    this.name = name;
  }
}

var p = new person("David", 21);
p.changeName("John");
//Now p.name equals to "John"
```

- The changeName method changes the object's name property to its argument.
- You can also define the function outside of the constructor function and associate it with the object.
```JavaScript
function person(name, age) {
  this.name= name;  
  this.age = age;
  this.yearOfBirth = bornYear;
}
function bornYear() {
  return 2016 - this.age;
}
```

- Note that it's not necessary to write the function's parentheses when assigning it to an object.
- Here is another example...
```JavaScript
function person(name, age) {
  this.name = name;  
  this.age = age;
  this.yearOfBirth = bornYear;
}
function bornYear() {
  return 2016 - this.age;
}

var p = new person("A", 22);
document.write(p.yearOfBirth());
// Outputs 1994
```

- Call the method by the property name you specified in the constructor function, rather than the function name.
- Declaring an array...
```JavaScript
var courses = new Array("HTML", "CSS", "JS");
```

- Declaring and modifying an array...
```JavaScript
var courses = new Array("HTML", "CSS", "JS");
var course = courses[0]; // HTML
courses[1] = "C++"; //Changes the second element
```

- Accessing an element outside of the array returns *undefined*.
```JavaScript
var courses = new Array("HTML", "CSS", "JS");
document.write(courses[10]);
//Outputs "undefined"
```

- The fastest way I know of how to create an array...
```JavaScript
var courses = ["HTML", "CSS", "JS"];
```

- In regards to associative arrays, JavaScript does not support arrays with named indexes
```JavaScript
var person = []; //empty array
person["name"] = "John";
person["age"] = 46;
document.write(person["age"]);
//Outputs "46"
```

- In JavaScript, arrays always use numbered indexes. It is better to use an object when you want the index to be a string (text). Use an array when you want the index to be a number. If you use a named index, JavaScript will redefine the array to a standard object.

- The math object allows us to perform mathematical tasks. This would produce pi `document.write(Math.PI); //Outputs 3.141592653589793`.
- Math has no constructor. There's no need to create a Math object first.
- To get a random number between 1-10, use Math.random(), which gives you a number between 0-1. Then multiply the number by 10, and then take Math.ceil() from it: Math.ceil(Math.random() * 10).
- This will ask a user for a number the produce the square root...
```JavaScript
var n = prompt("Enter a number", "");
var answer = Math.sqrt(n);
alert("The square root of " + n + " is " + answer);
```

- The setInterval() method calls a function or evaluates an expression at specified intervals (in milliseconds).
- It will continue calling the function until clearInterval() is called or the window is closed.
```JavaScript
function myAlert() {
   alert("Hi");
}
setInterval(myAlert, 3000);
```

- The Date object enables us to work with dates. A date consists of a year, a month, a day, an hour, a minute, a second, and milliseconds. Using new Date(), create a new date object with the current date and time.
```JavaScript
var d = new Date();
//d stores the current date and time
```

- Here are some date examples..
```JavaScript
//Fri Jan 02 1970 00:00:00
var d1 = new Date(86400000);

//Fri Jan 02 2015 10:42:00
var d2 = new Date("January 2, 2015 10:42:00");

//Sat Jun 11 1988 11:42:00
var d3 = new Date(88,5,11,11,42,0,0);
```

- JavaScript counts months from 0 to 11. January is 0, and December is 11.
Date objects are static, rather than dynamic. The computer time is ticking, but date objects don't change, once created.
- After a date object is created, one could format it like so...
```JavaScript
var d = new Date();
var hours = d.getHours();
//hours is equal to the current hour
```

- This prints the time to the browser every second...
```JavaScript
function printTime() {
  var d = new Date();
  var hours = d.getHours();
  var mins = d.getMinutes();
  var secs = d.getSeconds();
  document.body.innerHTML = hours+":"+mins+":"+secs;
}
setInterval(printTime, 1000);
```

- We declared a function printTime(), which gets the current time from the date object, and prints it to the screen.
- We then called the function once every second, using the setInterval method. The innerHTML property sets or returns the HTML content of an element. In our case, we are changing the HTML content of our document's body. This overwrites the content every second, instead of printing it repeatedly to the screen.

#### Bloc.io

**Today's Progress:**
None.


### R1D57 20181204
#### freeCodeCamp

**Today's Progress:**
None.

#### SoloLearn

**Today's Progress:**
Learned more about the DOM.
- The DOM represents a document as a tree structure.
- HTML elements become interrelated nodes in the tree.
- All those nodes in the tree have some kind of relations among each other.
- Nodes can have child nodes. Nodes on the same tree level are called siblings.
- There is a predefined document object in JavaScript, which can be used to access all elements on the DOM.
- As body is an element of the DOM, we can access it using the document object and change the content of the innerHTML property. `document.body.innerHTML = "Some text";`
- All HTML elements are objects. And as we know every object has properties and methods.
```JavaScript
//finds element by id
document.getElementById(id)

//finds elements by class name
document.getElementsByClassName(name)

//finds elements by tag name
document.getElementsByTagName(name)
```

- In the example below, the getElementById method is used to select the element with id="demo" and change its content:
```JavaScript
var elem = document.getElementById("demo");
elem.innerHTML = "Hello World!";
```

- The example above assumes that the HTML contains an element with id="demo", for example <div id="demo"></div>.
- The following example gets all paragraph elements of the page and changes their content:
```JavaScript
<p>hi</p>
<p>hello</p>
<p>hi</p>
<script>
var arr = document.getElementsByTagName("p");
for (var x = 0; x < arr.length; x++) {
  arr[x].innerHTML = "Hi there";
}
</script>
```

- The above script will result in the following HTML:
```HTML
<p>Hi there</p>
<p>Hi there</p>
<p>Hi there</p>
```

- Each element in the DOM has a set of properties and methods that provide information about their relationships in the DOM:
>element.childNodes returns an array of an element's child nodes.
element.firstChild returns the first child node of an element.
element.lastChild returns the last child node of an element.
element.hasChildNodes returns true if an element has any child nodes, otherwise false.
element.nextSibling returns the next node at the same tree level.
element.previousSibling returns the previous node at the same tree level.
element.parentNode returns the parent node of an element.

- We can, for example, select all child nodes of an element and change their content:
```JavaScript
<html>
  <body>
    <div id ="demo">
      <p>some text</p>
      <p>some other text</p>
    </div>

    <script>
     var a = document.getElementById("demo");
     var arr = a.childNodes;
     for(var x=0;x<arr.length;x++) {
       arr[x].innerHTML = "new text";
     }
    </script>

  </body>
</html>
```

- A `src` tag can be changed with JavaScript like so...
```JavaScript
<img id="myimg" src="orange.png" alt="" />
<script>
var el = document.getElementById("myimg");
el.src = "apple.png";
</script>
```

- A `href` attribute can also be changed like so...
```JavaScript
<a href="http://www.example.com">Some link</a>
<script>
var el = document.getElementsByTagName("a");
el[0].href = "http://www.sololearn.com";
</script>
```

- The style of HTML elements can also be changed using JavaScript.
```JavaScript
<div id="demo" style="width:200px">some text</div>
<script>
  var x = document.getElementById("demo");
  x.style.color = "6600FF";
  x.style.width = "100px";
</script>
```

- All CSS properties can be set and modified using JavaScript. Just remember, that you cannot use dashes (-) in the property names: these are replaced with camelCase versions, where the compound words begin with a capital letter. For example: the background-color property should be referred to as backgroundColor.

#### Bloc.io

**Today's Progress:**
None.


### R1D58 20181206
#### freeCodeCamp

**Today's Progress:**
None.

#### SoloLearn

**Today's Progress:**
*Creating Elements*
- element.cloneNode() clones an element and returns the resulting node.
- document.createElement(element) creates a new element node.
- document.createTextNode(text) creates a new text node.

For example:
`var node = document.createTextNode("Some new text");`

This will create a new text node, but it will not appear in the document until you append it to an existing element with one of the following methods:
- element.appendChild(newNode) adds a new child node to an element as the last child node.
- element.insertBefore(node1, node2) inserts node1 as a child before node2.

Another example:
```JavaScript
<div id ="demo">some content</div>

<script>
  //creating a new paragraph
  var p = document.createElement("p");
  var node = document.createTextNode("Some new text");
  //adding the text to the paragraph
  p.appendChild(node);

  var div = document.getElementById("demo");
  //adding the paragraph to the div
  div.appendChild(p);
</script>
```

*Removing Elements*
To remove an HTML element, you must select the parent of the element and use the removeChild(node) method.
```JavaScript
<div id="demo">
  <p id="p1">This is a paragraph.</p>
  <p id="p2">This is another paragraph.</p>
</div>

<script>
var parent = document.getElementById("demo");
var child = document.getElementById("p1");
parent.removeChild(child);
</script>
```

This removes the paragraph with id="p1" from the page.

>An alternative way of achieving the same result would be the use of the parentNode property to get the parent of the element we want to remove:
var child = document.getElementById("p1");
child.parentNode.removeChild(child);

*Replacing Elements*
To replace an HTML element, the element.replaceChild(newNode, oldNode) method is used.

```JavaScript
<div id="demo">
  <p id="p1">This is a paragraph.</p>
  <p id="p2">This is another paragraph.</p>
</div>

<script>
var p = document.createElement("p");
var node = document.createTextNode("This is new");
p.appendChild(node);

var parent = document.getElementById("demo");
var child = document.getElementById("p1");
parent.replaceChild(p, child);
</script>
```

>The code above creates a new paragraph element that replaces the existing p1 paragraph.

#### Bloc.io

**Today's Progress:**
None.


### R1D59 20181220
#### freeCodeCamp

**Today's Progress:**
None.

#### SoloLearn

**Today's Progress:**
In creating animations, I can start with this box...
```JavaScript
<style>
#container {
  width: 200px;
  height: 200px;
  background: green;
  position: relative;
}
#box {
  width: 50px;
  height: 50px;
  background: red;
  position: absolute;
}
</style>
<div id="container">
   <div id="box"> </div>
</div>
```

- In order to create an animation, the `setInterval()` method can be used to create a timer and call a function repeatedly like so `var t = setInterval(move, 500);`
- Now that the `move()` function is created, it needs to be defined...
```JavaScript
// starting position
var pos = 0;
//our box element
var box = document.getElementById("box");

function move() {
  pos += 1;
  box.style.left = pos+"px"; //px = pixels
}
```
- Once a function has been called for animation, it needs to be stopped otherwise it will just continue. `var t = setInterval(move, 10);`
```JavaScript
var pos = 0;
//our box element
var box = document.getElementById("box");
var t = setInterval(move, 10);

function move() {
  if(pos >= 150) {
    clearInterval(t);
  }
  else {
    pos += 1;
    box.style.left = pos+"px";
  }
}
```

#### Bloc.io

**Today's Progress:**
None.


### R1D60 20181225
#### freeCodeCamp

**Today's Progress:**
None.

#### SoloLearn

**Today's Progress:**
3 ways of declaring variables...
```JavaScript
var a = 10;
const b = 'hello';
let c = true;
```

- One of the best uses for `let` is in loops.
>let is not subject to Variable Hoisting, which means that let declarations do not move to the top of the current execution context.

- `const` variables have the same scope as variables declared using let. The difference is that const variables are immutable - they are not allowed to be reassigned.
>const is not subject to Variable Hoisting too, which means that const declarations do not move to the top of the current execution context.
Also note that ES6 code will run only in browsers that support it. Older devices and browsers that do not support ES6 will return a syntax error.

- This code...
```JavaScript
let name = 'David';
let msg = 'Welcome ' + name + '!';
console.log(msg);
```

..can be written as this..
```JavaScript
let name = 'David';
let msg = `Welcome ${name}!`;
console.log(msg);
```

>Notice, that template literals are enclosed by the backtick (` `) character instead of double or single quotes.
The ${expression} is a placeholder, and can include any expression, which will get evaluated and inserted into the template literal.

>To escape a backtick in a template literal, put a backslash \ before the backtick.

#### Bloc.io

**Today's Progress:**
Studied implementations of MinHeap.

#### Ruby Cookbook

**Today's Progress:**

Learned about `prepend`, `bsearch` and the different ways of working with strings.  I really liked this code on figuring out the class hierarchy...

```Ruby
module MyHelper
  def save
    puts "before"
    super
    puts "after"
  end
end

class MyGoodClass
  prepend MyHelper

  def save
    puts "my code"
  end
end

MyGoodClass.new.save

def parents(obj)
  ((obj.superclass ? parents(obj.superclass) : []) << obj).reverse
end

parents(MyGoodClass)
# => [Class, Object, BasicObject, Module]
```

### R1D61 20181226
#### freeCodeCamp

**Today's Progress:**
None.

#### SoloLearn

**Today's Progress:**
- In JavaScript we commonly use the for loop to iterate over values in a list:
```JavaScript
let arr = [1, 2, 3];
for (let k = 0; k < arr.length; k++) {
  console.log(arr[k]);
}
```

- The for...in loop is intended for iterating over the enumerable keys of an object. For example:
```JavaScript
let obj = {a: 1, b: 2, c: 3};
for (let v in obj) {
  console.log(v);
}
```

>The for...in loop should NOT be used to iterate over arrays because, depending on the JavaScript engine, it could iterate in an arbitrary order. Also, the iterating variable is a string, not a number, so if you try to do any math with the variable, you'll be performing string concatenation instead of addition.

- ES6 introduces the new for...of loop, which creates a loop iterating over iterable objects. For example:
```JavaScript
let list = ["x", "y", "z"];
for (let val of list) {
  console.log(val);
}
```

- The for...of loop works for other iterable objects as well, including strings:
```JavaScript
for (let ch of "Hello") {
  console.log(ch);
}
```

>The for...of loop also works on the newly introduced collections (Map, Set, WeakMap, and WeakSet).

- Old way of writing functions..
```JavaScript
function add(x, y) {
  var sum = x+y;  
  console.log(sum);
}
```

- New way of writing functions..
```JavaScript
const add = (x, y) => {
  let sum = x + y;  
  console.log(sum);
}
```

- Also can be written like this... `const greet = x => "Welcome " + x;`
- If no parameters, use this syntax... `const x = () => alert("Hi");`

This code...
```JavaScript
var arr = [2, 3, 7, 8];

arr.forEach(function(el) {
  console.log(el * 2);
});
```

..can be rewritten as follows..

```JavaScript
const arr = [2, 3, 7, 8];

arr.forEach(v => {
  console.log(v * 2);
});
```

- It is possible to create default values as parameters...
```JavaScript
function test(a, b = 3, c = 42) {
  return a + b + c;
}
console.log(test(5)); //50
```

..and in an arrow function as well..
```JavaScript
const test = (a, b = 3, c = 42) => {
  return a + b + c;
}
console.log(test(5)); //50
```

#### Bloc.io

**Today's Progress:**
None.

#### Ruby Cookbook

**Today's Progress:**
Covered creating and invoking a block, writing a method that accepts a block, binding a block argument to a variable.


### R1D62 20181227
#### freeCodeCamp

**Today's Progress:**
None.

#### SoloLearn

**Today's Progress:**
- The method definition shorthand does not require the colon or function keyword, as in the grow function of the tree object declaration...
```JavaScript
let tree = {
  height: 10,
  color: 'green',
  grow() {
    this.height += 2;
  }
};
tree.grow();
console.log(tree.height); // 12
```

- You can also use a property value shorthand when initializing properties with a variable by the same name.
```JavaScript
let height = 5;
let health = 100;

let athlete = {
  height,
  health
};
```

- When creating an object by using duplicate property names, the last property will overwrite the prior ones of the same name.  `var a = {x: 1, x: 2, x: 3, x: 4}`

>Duplicate property names generated a SyntaxError in ES5 when using strict mode. However, ES6 removed this limitation.

- With ES6, you can now use computed property names. Using the square bracket notation [], we can use an expression for a property name, including concatenating strings.
```JavaScript
// Example 1
let prop = 'name';
let id = '1234';
let mobile = '08923';

let user = {
  [prop]: 'Jack',
  [`user_${id}`]: `${mobile}`
};

// Example 2
var i = 0;
var a = {
  ['foo' + ++i]: i,
  ['foo' + ++i]: i,
  ['foo' + ++i]: i
};

// Example 3
var param = 'size';
var config = {
  [param]: 12,
  ['mobile' + param.charAt(0).toUpperCase() + param.slice(1)]: 4
};
console.log(config);
```

>It is very useful when you need to create custom objects based on some variables.

- ES6 adds a new Object method assign() that allows us to combine multiple sources into one target to create a single new object. Object.assign() is also useful for creating a duplicate of an existing object.
```JavaScript
let person = {
  name: 'Jack',
  age: 18,
  sex: 'male'
};
let student = {
  name: 'Bob',
  age: 20,
  xp: '2'
};
let newStudent = Object.assign({}, person, student);
```

- Here we used Object.assign() where the first parameter is the target object you want to apply new properties to. Every parameter after the first will be used as sources for the target. There are no limitations on the number of source parameters. However, order is important because properties in the second parameter will be overridden by properties of the same name in third parameter, and so on.
- In the following example, assignment was used to try to generate a new object. However, using = creates a reference to the base object. Because of this reference, changes intended for a new object mutate the original object:
```JavaScript
let person = {
  name: 'Jack',
  age: 18
};

let newPerson = person; //  newPerson references person
newPerson.name = 'Bob';

console.log(person.name); // Bob
console.log(newPerson.name); // Bob
```

- To avoid this (mutations), use Object.assign() to create a new object
```JavaScript
let person = {
  name: 'Jack',
  age: 18
};

let newPerson = Object.assign({}, person);
newPerson.name = 'Bob';

console.log(person.name); // Jack
console.log(newPerson.name); // Bob
```

- Finally, you can assign a value to an object property in the Object.assign() statement.
```JavaScript
let person = {
  name: 'Jack',
  age: 18
};

let newPerson = Object.assign({}, person, {name: 'Bob'});
```

- What is the output of this code?
```JavaScript
const obj1 = {
  a: 0,
  b: 2,
  c: 4
};
const obj2 = Object.assign({c: 5, d: 6}, obj1);
console.log(obj2.c, obj2.d);
// 4 6
```

#### Bloc.io

**Today's Progress:**
None.

#### Ruby Cookbook reading
Learned about...
- Outside variables within a code block.
- Writing an iterator over a data structure.
- Using symbols as hash keys
- Creating a Hash with a default value


### R1D63 20181228
#### freeCodeCamp

**Today's Progress:**
None.

#### SoloLearn

**Today's Progress:**
- Destructuring an array. The following example demonstrates how to unpack the elements of an array into distinct variables..
```JavaScript
let arr = ['1', '2', '3'];
let [one, two, three] = arr;

console.log(one); // 1
console.log(two); // 2
console.log(three); // 3
```

- We can use also destructure an array returned by a function.
```JavaScript
let a = () => {
  return [1, 3, 2];
};

let [one, , two] = a();
```

- Notice that we left the second argument's place empty. The destructuring syntax also simplifies assignment and swapping values..
```JavaScript
let a, b, c = 4, d = 8;
[a, b = 6] = [2]; // a = 2, b = 6

[c, d] = [d, c]; // c = 8, d = 4
```

- What is the output of the following code?
```
let names = ['John', 'Fred', 'Ann'];
let [Ann, Fred, John] = names;
console.log(John);
```

Ann

- Similar to Array destructuring, Object destructuring unpacks properties into distinct variables.
```JavaScript
let obj = {h:100, s: true};
let {h, s} = obj;

console.log(h); // 100
console.log(s); // true
```

- We can assign without declaration, but there are some syntax requirements for that:
```JavaScript
let a, b;
({a, b} = {a: 'Hello ', b: 'Jack'});

console.log(a + b); // Hello Jack
```

- The () with a semicolon (;) at the end are mandatory when destructuring without a declaration. However, you can also do it as follows where the () are not required..
```JavaScript
let {a, b} = {a: 'Hello ', b: 'Jack'};
console.log(a + b);
```

- Can also assign the object to new variable names..
```JavaScript
var o = {h: 42, s: true};
var {h: foo, s: bar} = o;

//console.log(h); // Error
console.log(foo); // 42
```

- Finally you can assign default values to variables, in case the value unpacked from the object is undefined.
```JavaScript
var obj = {id: 42, name: "Jack"};

let {id = 10, age = 20} = obj;

console.log(id); // 42
console.log(age); // 20
```

- What is the output of the following code?
```JavaScript
const obj = {one: 1, two: 2};
let {one:first, two:second} = obj;
console.log(one);
```

Error

#### Bloc.io

**Today's Progress:**
None.

#### Ruby Cookbook
- Adding elements to a hash in different ways.


### R1D64 20190102
#### freeCodeCamp

**Today's Progress:**
None.

#### SoloLearn

**Today's Progress:**
- Write a function that checks if an array contains all the arguments passed..
```JavaScript
function containsAll(arr) {
  for (let k = 1; k < arguments.length; k++) {
    let num = arguments[k];
    if (arr.indexOf(num) === -1) {
      return false;
    }
  }
  return true;
}
let x = [2, 4, 6, 7];
console.log(containsAll(x, 2, 4, 7));
console.log(containsAll(x, 6, 4, 9));
```

- While this does the job, ES6 provides a more readable syntax to achieve variable number of parameters by using a rest parameter..
```JavaScript
function containsAll(arr, ...nums) {
  for (let num of nums) {
    if (arr.indexOf(num) === -1) {
      return false;
    }
  }
  return true;
}
```

- The ...nums parameter is called a rest parameter. It takes all the "extra" arguments passed to the function. The three dots (...) are called the Spread operator.

> Only the last parameter of a function may be marked as a rest parameter. If there are no extra arguments, the rest parameter will simply be an empty array; the rest parameter will never be undefined.

- What is the output of the following code?
```JavaScript
function magic(...nums) {
  let sum = 0;
  nums.filter(n => n % 2 == 0).map(el => sum+= el);
  return sum;
}
console.log(magic(1, 2, 3, 4, 5, 6));  // 12
```

- It is common to pass the elements of an array as arguments to a function. Before ES6, we used the following method..
```JavaScript
function myFunction(w, x, y, z) {
  console.log(w + x + y + z);
}
var args = [1, 2, 3];
myFunction.apply(null, args.concat(4));
```

- ES6 provides an easy way to do the example above with spread operators..
```JavaScript
const myFunction = (w, x, y, z) => {
  console.log(w + x + y + z);
};
let args = [1, 2, 3];
myFunction(...args, 4);
```

- Spread in array literals = Before ES6, we used the following syntax to add an item at middle of an array..
```JavaScript
var arr = ["One", "Two", "Five"];

arr.splice(2, 0, "Three");
arr.splice(3, 0, "Four");
console.log(arr);
```

- However, in ES6 the spread operator lets us do this more easily..
```JavaScript
let newArr = ['Three', 'Four'];
let arr = ['One', 'Two', ...newArr, 'Five'];
console.log(arr);
```

- In objects it copies the own enumerable properties from the provided object onto a new object..
```JavaScript
const obj1 = { foo: 'bar', x: 42 };
const obj2 = { foo: 'baz', y: 5 };

const clonedObj = {...obj1}; // { foo: "bar", x: 42 }
const mergedObj = {...obj1, ...obj2}; // { foo: "baz", x: 42, y: 5 }
```

- However, if you try to merge them you will not get the result you expected..
```JavaScript
const obj1 = { foo: 'bar', x: 42 };
const obj2 = { foo: 'baz', y: 5 };
const merge = (...objects) => ({...objects});

let mergedObj = merge(obj1, obj2);
// { 0: { foo: 'bar', x: 42 }, 1: { foo: 'baz', y: 5 } }

let mergedObj2 = merge({}, obj1, obj2);
// { 0: {}, 1: { foo: 'bar', x: 42 }, 2: { foo: 'baz', y: 5 } }
```

> Shallow cloning or merging objects is possible with another operator called Object.assign().

- What is the output of the following code?
```JavaScript
let nums = [3, 4, 5];
let all = [1, 2, ...nums, 6];
console.log(all[3]); // 4
```

#### Bloc.io

**Today's Progress:**
Still trying to learn how to do an insert and find in a min heap.

#### Ruby Cookbook

- Learned how to remove elements from a hash.


### R1D65 20190104
#### freeCodeCamp

**Today's Progress:**
None.

#### SoloLearn

**Today's Progress:**
None.

#### Bloc.io

**Today's Progress:**
Studying implementation of inserting data into a tree structure.


### R1D66 20190116
#### freeCodeCamp

**Today's Progress:**
None.

#### SoloLearn

**Today's Progress:**
None.

#### Bloc.io

**Today's Progress:**
Made significant progress on my tree assignment. Need to figure out how to get past a..
```
NoMethodError:
       undefined method `rating' for nil:NilClass
     # ./min_heap.rb:11:in `insert'
     # ./min_heap.rb:13:in `insert'
     # ./min_heap_spec.rb:23:in `block (3 levels) in <top (required)>'
```

..error.

### R1D67 20190226

#### Bloc.io

**Today's Progress:**
Completed section on alternative active record library made from scratch.  Specifically inserted code that performs database updates.


### R1D68 20190227

#### Bloc.io

**Today's Progress:**
Trying to add more functionality to my ORM project.  Specifically adding code to update multiple records and using `method_missing` to add support for dynamic `update_*` method calls.


### R1D69 20190302

#### Bloc.io

**Today's Progress:**
- Added functionality to insert a hash of values to my active record replacement.
- Implemented  `method_missing` for dynamic `update_*` calls.
- Added a `take`, `where` and `not` instance methods.


### R1D69 20190228
#### freeCodeCamp

**Today's Progress:**

**Thoughts/Notes:**

**Link to work:**

#### SoloLearn

**Today's Progress:**

#### Bloc.io

**Today's Progress:**

**Thoughts/Notes:**

**Link to work:**

### R1D69 20190228
#### freeCodeCamp

**Today's Progress:**

**Thoughts/Notes:**

**Link to work:**

#### SoloLearn

**Today's Progress:**

#### Bloc.io

**Today's Progress:**

**Thoughts/Notes:**

**Link to work:**
