# #100DaysOfCode Log - Round 2

My second log of my #100DaysOfCode challenge. First round started on August 3rd, 2017.

## Log

### R2D1 20190809
#### Udemy
Learned that these 3 lines are the same..

```ruby
p 10 / 5
p 10./(5)
p 10.div(5)
```

Glad I stuck with listening to the basics on this udemy course.  I had no idea about the second and third line.  It wasn't taught in any of the beginners courses I took before.


### R2D2 20190810
#### udemy

I wanted my Star Wars day to be memorable and it kind of was given I'm trying to learn more about Docker so that I can setup an Eclipse Che environment or figure out how to get a free Cloud9 AWS account to start an actual Rails project.

I learned more of the basic stuff in the Learn to Code with Ruby course.  Really nothing new there in the material I was able to get through today.



### R2D3 20190812
#### udemy

I'm still following along with the Learn to Code with Ruby class.  I'm still watching it 2x because I know most everything they are going over.

There is a method that I skimmed by before in a tutorial or maybe I saw it in a book which is the `respond_to?` method. I've never seen examples of it the way I saw it in the video. It's pretty cool in that it can be used to help clean or check on data before it's used or consumed.

Here are some examples..
```Ruby
if num.respond_to?("length") # false won't run
  num.next
end
puts
puts "Hello".respond_to?("length")
puts "Hello".respond_to?("class")
puts "Hello".respond_to?("upcase")
puts "Hello".respond_to?("odd?")
puts
# Using a symbol instead
puts "Hello".respond_to?(:length)
puts "Hello".respond_to?(:downcase)
puts 1.respond_to?(:next)
# Using the symbol object takes up less memory in Ruby
```



### R2D4 20190813
#### udemy

**Today's Progress:**
Made more progress through the Ruby course.  Learned a few things about ranges and `rand`.  I even had another opportunity to code out another "FizzBuzz" challenge.


### R2D5 20190814
#### freeCodeCamp

**Today's Progress:**
I almost have my first project done which is the tribute page.  Hopefully I can finish a second by tomorrow night.

#### Udemy

**Today's Progress:**
Completed 2 basic HTML classes, a database design course and more progress with the Ruby coding course.



### R2D6 20190819
#### udemy

**Today's Progress:**
Listened to more of the database design classes and made more progress on the Learn to Code with Ruby class.

**Thoughts/Notes:**
It's weird how some of the ruby functions normally return what you would expect but there are a few like `.pop` where if you call that method with a 1 as a parameter, it will return the value as an array.  If you don't use the parameter and assign it to a variable, you can see that it will just return the value.


### R2D7 20190820
#### udemy

**Today's Progress:**
Completed the udemy databae design class.  Continued on with the udemy Ruby course. This Ruby course is a long one.  Just to break things up, I started the Learn Responsive Web Development from Scratch course.  See notes below.

**Thoughts/Notes:**
A fluid layout example could be...
- 90% width on the header
- 3 body sections
  - 50% width
  - 20% width
  - 20% width
  - 5% padding in between them

Use flexible images so that they scale down and not go outside their container.

Use percentages when sizing images. Use different percentages depending on screen size.

```css
img {
  max-width: 100%;
}
```

The @media rule has actually been around awhile. It will allow multiple stylesheets which would be one for each type of document. The most popular are "screen" and "print". Some of the others include braille, handheld, projection and tv.

Examples of using media queries with external stylesheets..
- `<link rel="stylesheet" media="screen" href="style.css" />`
- `<link rel="stylesheet" media="only screen and (min-width:320px) and (max-width:568px)" href="mobile.css" />`
- `<link rel="stylesheet" media="only screen and (min-width:768px) and (max-width:980px)" href="tablet.css" />`

Here is some actual syntax..
```css
@media(max-width: 600px) {
  /* Styles go here */
}

@media(max_width: 700px) {
  /* Styles go here */
}

@media only screen and (min-width: 320px) and (max-max_width: 568px) {
  /* Styles go here */
}

@media only screen and (min-width: 768px) and (max-width: 980px) {
  /* Styles go here */
}
```

Whenever there is a breakpoint (where the screen gets smaller) we can have a CSS transition to make it look smoother.

```css
#main-column{
  transition: width 2s;
}
```

The "width" is the CSS property we want to animate and the "2s" is the duration in seconds.


### R2D8 20190821
#### udemy

**Today's Progress:**
Went through some more videos on Ruby as well as a responsive web design.

**Thoughts/Notes:**
Just figured out the responsive web design class is 6 years old so there is no flexbox or grid usage but still, I like the parts about the `@media` queries.


### R2D9 20190823
#### Misc

**Today's Progress:**
Old laptop broke. Spent the entire evening last night setting up new/refurb laptop. I can't believe it takes that long. Still have to setup Ruby on Rails, Git, Nodejs and install my Atom editor packages and a few other things.


### R2D10 20190826
#### udemy

**Today's Progress:**
Completed a 4 hour responsive web design course on Udemy and made more progress on the Learn to Code in Ruby Udemy course.


### R2D11 20190827
#### udemy

**Today's Progress:**
Watched more Ruby video's so that I can get a better grasp of the syntax. I also completed an HTML5 and CSS3 video series on udemy.

#### Misc

**Today's Progress:**
Trying to decide on colors and a layout for a family members website redesign.  Currently it's over 10 years old and hasn't been touched in 10 years.


### R2D12 20190829
#### udemy

**Today's Progress:**
Made more progress with the Ruby course on Udemy.  Learned about `.map` and `.collect`.


### R2D13 20190901
#### udemy

**Today's Progress:**
Had a review on some methods in the Ruby Udemy course on `concat`, `break`, `include?`, `index` and `find_index`, `select`, `reject` and `sort`.

I feel this is a really good review because I was not taught about any of these methods in the coding camp.

#### SoloLearn

**Today's Progress:**
It had been awhile since I had looked at JavaScript but it came back to me when doing a review in SoloLearn.  I'm trying to finish the JavaScript module soon.



### R2D14 20190902
#### Udemy

**Today's Progress:**
Worked on some front end courses and even watched an Adobe XD set of videos to play around with it to see if it will be of use in the future.



### R2D15 20190904
#### Udemy

**Today's Progress:**
Started a CSS course and completed the AdobeXD mini course.



### R2D16 20190909
#### udemy

**Today's Progress:**
Worked on more CSS with a Udemy course



### R2D17 20190910
#### udemy

**Today's Progress:**
Watched more CSS videos and all of it was review.



### R2D18 20190911
#### udemy

**Today's Progress:**
Finally learning some CSS that I've never seen in other tutorials by studying 'combinators'.

- Adjacent Sibling
`div + p {}`
This only applies css where a p tag immediately follows an h2 tag.
Example..

```CSS
h2 + p {
  color: red;
}
```

```HTML
<div>
  <h2>not applied</h2>
  <p>css applied</p>
  <h2>not applied</h2>
  <h3>not applied</h3>
  <p>not applied</p>
  <h2>not applied</h2>
  <p>css applied</p>
</div>
```

- General Sibling
`div ~ p {}`
  1. Has to have the same parent.
  2. Second element comes after first.
Example..
```CSS
h2 ~ p {
  color: red;
}
```

```HTML
<div>
  <h2>not applied</h2>
  <p>css applied</p>
  <h2>not applied</h2>
  <h3>not applied</h3>
  <p>css applied</p>
</div>
```

- Child
`div > p {}`
  1. Second element is a direct child of first element.
Example..
```CSS
div > p {
  color: red;
}
```

```HTML
<div>
  <div>not applied</div>
  <p>css applied</p>
  <div>not applied</div>
  <article>
    <p>not applied</p>
  </article>
  <p>css applied</p>
</div>
```

- Descendant
`div p {}`
1. Second element is a descendant of the first element
Example..
```CSS
div p {
  color: red;
}
```

```HTML
<div>
  <div>not applied</div>
  <p>css applied</p>
  <div>not applied</div>
  <article>
    <p>css applied</p>
  </article>
  <p>css applied</p>
</div>
```



### R2D19 20190912
#### udemy

**Today's Progress:**
Completed a 2 hour video on CSS. Made more progress through what's turning out to be another pretty cool CSS course.

**Thoughts/Notes:**
*Margin Collapsing* is when to elements are right next to each other and the margin of the joining sides over lap.  If one elements margin is bigger than the other, that margin is used instead of the smaller margin.

_Body has a margin value_ - When trying to measure things within the body where you need exact measurements to fit the entire screen, know that the body has a margin by default.


#### The Odin Project

**Today's Progress:**
Had to reset up some stuff that was setup on previous laptop.  Good to touch rails again.



### R2D20 20190916
#### Udemy

**Today's Progress:**
Made some more progress on the Ruby course.  I love the small examples and the short challenges he gives.


#### The Odin Project

**Today's Progress:**
Did a review on Git and flew through some of the SQL material given I work with that every day.  

This gitignore website seems like it could come in handy..

(https://www.gitignore.io/)[https://www.gitignore.io/]

I think I'll probably be able to fly through the HTML/CSS section along with at least half of the Ruby section.



### R2D21 20190917
#### udemy

**Today's Progress:**
Changed things up today.  Started a short 2+ hour Udemy tutorial titled "Build a Responsive Website with a Modern Flat Design".  Looks like I'm going to be learning about the Foundation Framework.

#### The Odin Project

**Today's Progress:**
I can't believe the heavy emphasis on Git that The Odin Project gives to it.  I'm almost done with the Git section. I think I'll finish it up tomorrow and then moving on to the front end section.


### R2D22 20190919
#### freeCodeCamp

**Today's Progress:**

**Thoughts/Notes:**

**Link to work:**

#### Denver Startup week

**Today's Progress:**
Attended GraphQL, pick your next database and React sessions


#### The Odin Project

**Today's Progress:**
Notes on how to write good commit Git messages...

1. Seperate subject from body with a blank line
2. Limit the subject line to 50 characters
3. Captialize the subject line
4. Do not end the subject line with a period
5. Use the imperative mood in the subject line
6. Wrap the body at 72 characters
7. Use the body to explain what and why vs how

A properly formed Git commit subject line should always be able to complete the following sentence:

- If applied, this commit will _your subject line here_

For example:

- If applied, this commit will *refactor subsystem X for readability*
- If applied, this commit will *update getting started documentation*
- If applied, this commit will *remove deprecated methods*
- If applied, this commit will *release version 1.0.0*
- If applied, this commit will *merge pull request #123 from user/branch*

This doesn't work like the way I've been doing it..

- If applied, this commit will *fixed bug with Y*
- If applied, this commit will *changing behavior of X*
- If applied, this commit will *more fixes for broken stuff*
- If applied, this commit will *sweet new API methods*

Here is an example for number 7...

```
commit eb0b56b19017ab5c16c745e6da39c53126924ed6
Author: Pieter Wuille <pieter.wuille@gmail.com>
Date:   Fri Aug 1 22:57:55 2014 +0200

   Simplify serialize.h's exception handling

   Remove the 'state' and 'exceptmask' from serialize.h's stream
   implementations, as well as related methods.

   As exceptmask always included 'failbit', and setstate was always
   called with bits = failbit, all it did was immediately raise an
   exception. Get rid of those variables, and replace the setstate
   with direct exception throwing (which also removes some dead
   code).

   As a result, good() is never reached after a failure (there are
   only 2 calls, one of which is in tests), and can just be replaced
   by !eof().

   fail(), clear(n) and exceptions() are just never called. Delete
   them.
```

Note: In most cases, you can leave out details about how a change has been made. Code is generally self-explanatory in this regard (and if the code is so complex that it needs to be explained in prose, that’s what source comments are for). Just focus on making clear the reasons why you made the change in the first place—the way things worked before the change (and what was wrong with that), the way they work now, and why you decided to solve it the way you did.




### R2D23 20190926
#### udemy

**Today's Progress:**
Started another course called 8 Beautiful Ruby on Rails apps.

**Thoughts/Notes:**
- Calling `5.methods` will give a list of all available methods for the number 5.

- Using symbols is more efficient in the following example...
```Ruby
"twelve".object_id
```
..vs using this..
```ruby
:twelve.object_id
```
- Started a project named Cabinet to store files.



### R2D24 20191002
#### udemy

**Today's Progress:**
Went thru more of the Rails projects lessons. Associated a docs table with a user table.


### R2D25 20191015
#### Udemy

**Today's Progress:**
I've already viewed the first project once. I'm going to go through it a second time but add some customizations to it.

**Thoughts/Notes:**
Steps starting with video 21..

1. Create static page named welcome.
* Used `rails generate controller welcome index`.  If you want to create a view file, you must create a controller file for it.  Adding `index` to that command adds index.html.erb file.
2. Entering `rails s` will start the rails server.
* Going to localhost:3000 will get you to the main page
* Going to localhost:3000/welcome/index will get you to a generic page. The welcome word is the controller and the index word is the action.
3. After modifying the /config/routes.rb file to `root 'welcome#index'`, that will make it so that all you have to do is enter localhost:3000 and it will go to the same page as localhost:3000/welcome/index
4. Added the `simple_form`, `haml` and `devise` gems then run `bundle install`
5. Renamed index.html.erb to index.html.haml
6. Generated a model called Doc with `rails generate model Doc title:string content:text` then performed a `rake db:migrate`. The schema.rb file only appears in /db/migrate after running the first `rake db:migrate` the first time. Never touch this file for any reason but rather use migrations.
7. Run `rails generate controller Docs` which creates the view directory but not the file.
8. Added `resources` to the routes.rb file for docs.
* If I go to the terminal, I can run `rake routes` to see all the new docs routes.
9. Added new view files to docs.. \_form.html.haml (which is a partial) and new.html.haml.
10. Actually install simple_form by going to the home page for instructions. Since the gem is installed, so all that is left is `rails generate simple_form:install`. After running that command, restart the rails server.
11. Modify the partial file that was created to list multiple document entries if they exist.
12. Enter `= render 'form'` in the new.html.haml file so that it can render the partial.
13. Modify the docs_controller.rb file so that it doesn't throw an error.
* At this point we can access localhost:3000/docs/new
14. Need to add a show view in order to show a doc entry.
* Add a `before_action` at the top of the controller to do a `find_doc` on `:show`, `:edit`, `:update` and `:destroy` (actions).
* When trying to go to /docs, I get a missing template error which is telling us that the view for the index action does not exist.
15. Add code to the docs controller for the index action.


#### The Odin Project

**Today's Progress:**
Reviewed the web page on how to write a good Git commit message.

(https://chris.beams.io/posts/git-commit/)[https://chris.beams.io/posts/git-commit/]

My plan is to use the guidance in this post to write my own messages for the Udemy project - FileCabinet.

#### Misc Notes
**Instructions for a new Git repo:**

Create a new repository on the command line where the name of the repo is `filecab`.

```github
echo "# filecab" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin git@github.com:jmuldvp/filecab.git
git push -u origin master
```

### R2D26 20191016
#### Udemy

**Today's Progress:**

**Thoughts/Notes:**

**Link to work:**

#### SoloLearn

**Today's Progress:**

#### The Odin Project

**Today's Progress:**



### R2D27 20191017
#### freeCodeCamp

**Today's Progress:**

**Thoughts/Notes:**

**Link to work:**

#### SoloLearn

**Today's Progress:**

#### The Odin Project

**Today's Progress:**



### R2D28 20191018
#### freeCodeCamp

**Today's Progress:**

**Thoughts/Notes:**

**Link to work:**

#### SoloLearn

**Today's Progress:**

#### The Odin Project

**Today's Progress:**



### R2D29 20191019
#### freeCodeCamp

**Today's Progress:**

**Thoughts/Notes:**

**Link to work:**

#### SoloLearn

**Today's Progress:**

#### The Odin Project

**Today's Progress:**



### R2D30 20191020
#### freeCodeCamp

**Today's Progress:**

**Thoughts/Notes:**

**Link to work:**

#### SoloLearn

**Today's Progress:**

#### The Odin Project

**Today's Progress:**
