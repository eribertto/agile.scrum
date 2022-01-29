After watching this video, you'll be able to define a user story, describe the
parts of a good user story, explain why adding acceptance criteria is important,
define the invest acronym, and describe an Epic and when to use it. So what is a
user story? Simply put, the user story represents a piece of business value that
the team can deliver within a done increment. We used to call these
requirements, but user stories are so much more. Requirement is usually, I need
this, I need that, but a user story includes: Who is it for? What do they need?
But very importantly, why do they need it? What is the business value that they
get out of getting this feature or function? So stories should contain a good
description of the business value: What it is. Who needs it? What is the value
that we get out of that story? Then, I like to have any assumptions, and any
details documented in the story. Sometimes, you know there are assumptions,
you're doing a story and it needs some kind of persistence. And you know you're
going to use a relational database, put that in there to give the developer a
hint, "Hey, don't go looking for NoSQL databases, we decided we're going to use
a relational database. So anything you know, any assumptions, we're going to
provision something in the cloud, put that in the user story, so that the
developer knows what your intentions are. And then most important, you need the
definition of done, some acceptance criteria. How do I know when this story is
complete? When it is done? You don't want to find out in the sprint review that
the the product owner says, "Hey, that's not what I wanted." You want to
document the definition of done to say, "Well, this is the definition we agreed
on. This is what the story does, and if it's not what you want, we can write
another story, but we did what they said it should do." So the story
description, what do you put in that description? Again, you want to document a
persona, requesting some functionality to get some goal or achieve some goal,
get some business value. And so the way that we do this is with this problem in
syntax as a role. What's the role? Is it the marketing manager? Is it the
customers? The sysadmin?  Right? Who is this for? And then I need some
functionality. What is it that they need? This is the meat of the user story,
but very importantly, so that I gain some business benefit. What is the benefit
of delivering that function? When we go back and we prioritize the backlog,
we're going to look at the business value as one of the criteria to say, "Should
this be high in the backlog or lower in the backlog?" So it's very, very
important, not only to have what it is, but what's the value that we get out of
it? Then there's assumptions and detail. So anything that you know, right, it
doesn't have to be in great detail. But anything you know, as I said, you know,
if you know that you're going to use a database, some persistence, you know,
just list it there. Anything you talked about while you're writing the story,
put that in. What you're trying to do is help the developer understand what
needs to be done; anything that wasn't obvious to get this story completed. And
then there's the acceptance criteria, the definition of done. This is
critically, critically important. Really important to understand what makes this
user story finished, complete or done. And for that we use a syntax called
Gherkin, named after the pickle. And Gherkin is a syntax that makes it easy for
stakeholders, customers, and developers alike to describe the definition of
done. To describe the behavior of the system. And it goes something like this.
Given some precondition, this sets up the story, given I have five items in my
shopping cart, right? Given I'm already logged into the system, given whatever
the given is, it sets up the story. And then what's the action that happens?
Right? What is the thing that triggers it, when this happens, when I add another
item to my cart, or I delete an item to my cart? And then finally, what is the
testable result of that? Then I should see this, I shouldn't see that, I should
have six items in my cart, or I should see four items in my cart, right? It
makes it very easy for everyone to understand. Given this is the is the base
case, when this happens, then I should have some measurable outcome. And if I
measure that outcome, the story is done. So let's look at a sample story. As a
marketing manager, now we know the role.  This is not for the customer. This is
not for the sysadmin. This is for the marketing manager, so we know who is going
to gain some benefit from this. I need a list of customer names and emails. So
now we know what the function is, they need to list out customers with their
emails, and then the business value, so that I can notify them of marketing
promotions. But now I can say, "How important is it to notify customers of
marketing promotions?" And maybe I put that before another story that is less
important. So now I've captured: Who is it for? What is it that I need? And why
do I need it? What value do I get from it? Then I like to put in any
assumptions. These assumptions help the developer in creating the code that goes
with the story. So one assumption is we maintain customer emails, maybe we
don't. Maybe this story has a dependency on another story that actually creates
the customer emails. Maybe there's another assumption: Customers have opted in
to promotions. That's kind of important.  Somebody might not have thought of
that. Hey, we can't just email all our customers, we have to allow them to opt
into getting promotions. And then we have the acceptance criteria. What is the
definition of done? What is the behavior that we want this story to have? And
we'll use that Gherkin syntax, given there are 100 customers in the database. So
that sets up the scenario.  And 90 have opted into email promotions. So this is
critically important is not just all 100, it's the 100 that have opted in to
email promotion, so now developers know they need to filter how many customers
in the database by who has opted in. When I request a customer email list, so
that is the action, that is the thing that happens, then I should see a list of
90 customer emails, not 100 customer emails, 90 customer emails, because only 90
opted in to the email promotion.  So you can see that this is something you
could give to a stakeholder, the marketing manager could understand the behavior
and say, "Yep, that is the behavior I want." The developer can read this and
say, "Yep, that's the behavior I can deliver." And that at the end of the
sprint, as long as when you ask for customers, you only get the ones who have
opted in. And that is the definition of done. And so there's no arguments about
whether the story is done or not. If it has that behavior, it's done. I'm not
much for acronyms, but Bill Wake has a pretty good one with INVEST. INVEST says,
"Stories should be independent, I want to be able to rank them in the backlog, I
want to be able to move them around, I want to be able to say that this one
comes before that one." Now I know they can't always be independent, sometimes
there are dependencies, right? In the previous example, we had an assumption
that there were customer emails in the database, and if there weren't, then that
wasn't an independent story, it was dependent on the story that put emails in
the database. But for the most part, you want to try to write them so that
they're independent. They also need to be negotiable, right? I'm going to move
them in the backlog. I'm going to rank them higher or lower. Maybe I'm going to
say we should put more value more functionality or less functionality to
negotiate how much really has to be done. So they should be negotiable. They
shouldn't be too tightly coupled to exactly what's needed. And then they need to
be valuable, right? I need to be able to say, "How valuable is this story? What
is what value does the customer get out of it, to make sure that it really is a
user story." And and not just a technical debt story that this is something I
need to do that the customer never sees. It needs to be estimable, I need to be
able to estimate it. How big is it? Small? Medium? Large? There has to be enough
information in there that I could say, "Wow, this is a really big story, given
everything that's in here." Alright. And it's not just one line that looks
simple, but then really becomes hard. And it should be small. You want it to be
something that someone can work on in a sprint, so it's got to be smaller than a
sprint. And then finally, it needs to be testable. I need to be able to test
whether that story is done. I want to test the definition of done for that
story. And so stories need to be testable. What about really big ideas? Well,
really big ideas are called Epics. We use epics anytime that we have a story
that is bigger than a single sprint, because the story must be smaller than a
sprint, by definition. And so when it's bigger, that becomes a big idea that we
can't get done in a sprint, so we make it Epic and then we add smaller stories
that make up the Epic to the Epic. So an Epic in the hierarchy is higher than a
story. Stories are consumed by Epics. And so usually any story that's too big,
we make it Epic, right? If we can't estimate it on its own, then we break it
down into smaller things that we can estimate. So when do we use an Epic? Well,
clearly, when a story is too large to put in a sprint, then we make it an Epic.
Usually backlog items will start out as big ideas, right?  They're they're
gonna, they're gonna be very large. And so they start out as Epics. And then as
we refine the backlog, we make them smaller and smaller stories that we can put
in a sprint.  And so for sprint planning, you want to break all of those big
stories up into smaller stories, break up all those Epics into smaller stories,
Things that usually come in the new issues, sometimes those are Epics, right.
Somebody asked for a feature or a function. It sounds pretty simple, but it's
going to take more than one sprint. And so you put it in as an Epic, and then
you break it down into user stories later. In this video, you learned that a
user story documents a persona requesting a function to achieve a goal. Using a
template helps ensure stories are complete. Defining done helps minimize
misunderstandings and well formed stories will meet the criteria of the INVEST
acronym. And Epics can be used to capture big ideas.