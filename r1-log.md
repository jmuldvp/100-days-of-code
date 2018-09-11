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

**Thoughts/Notes:**

**Link to work:**

#### SoloLearn

**Today's Progress:**

#### Bloc.io

**Today's Progress:**

**Thoughts/Notes:**

**Link to work:**

### R1D30 20180912
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
