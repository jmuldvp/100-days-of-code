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


### R1D3
#### freeCodeCamp

**Today's Progress:**

**Thoughts:**

**Link to work:**

#### Bloc.io

**Today's Progress:**

**Thoughts:**

**Link to work:**
<br />


### R1D4
#### freeCodeCamp

**Today's Progress:**

**Thoughts:**

**Link to work:**

#### Bloc.io

**Today's Progress:**

**Thoughts:**

**Link to work:**
