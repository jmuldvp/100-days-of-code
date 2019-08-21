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
#### freeCodeCamp

**Today's Progress:**

**Thoughts/Notes:**

**Link to work:**

#### SoloLearn

**Today's Progress:**

#### The Odin Project

**Today's Progress:**