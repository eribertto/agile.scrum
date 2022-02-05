After watching this video, you'll be able to describe the daily workflow,
determine which story you should work on next, and explain why you should not
work on more than one story at a time. In the steps in the scrum process, we've
gone all the way through backlog refinement and sprint backlog, and now we are
off to actually executing the sprint. So, the sprint is one iteration through
design, code, test, deploy, right?  It's one iteration through that whole cycle
and we do this in two-week increments.  And it's really important that every one
of them has a goal so everyone knows the goal that they're working for. So, the
daily execution, what each member wants to do is, when they start the sprint,
they take the next highest item off the sprint backlog that they have the skills
to work for. I realize that some UI developers can't do backend work, that's
fine, but the next item, the highest item, you don't get to pick one in the
middle, you don't get to pick your favorite item, you should be doing in the
order of business importance. The next highest thing in the sprint backlog, you
pull it off and you assign it to yourself. Very, very important to assign it to
yourself so everybody knows you're working on it. And then you move it into In
Progress so that now, visually, everybody can see that you're working on it.
So, let's go back to our Kanban board. We see we have three stories in the
sprint backlog and so, right now, we don't care about anything that is to the
left of the sprint backlog because we want to concentrate on the sprint backlog.
What's in process? What needs to be reviewed?  And what is going to get done?
So, right now, for your daily execution, you're going to take the next highest
thing on the sprint backlog, move it to In Process and open it up so that you
can assign it to yourself. So, once it opens up, you click on the assignees.
One of the cool things is that you can just click on a link that says Assign
Yourself, otherwise, you could drop down and assign it to someone else. But you
want to go assign it to whoever you are in GitHub. So, now I’ve just assigned
this to myself and GitHub, uh, so I can close that story or, obviously, I’m
going to read the story, understand what it is, understand what I have to do,
and then go close that story, and then it shows up in the In Progress column
with a little avatar. It happens to be the avatar that is, you know, my picture
on GitHub, but it's whatever your avatar is on GitHub, that's what it shows up.
So, look at what I can see here. Now anyone, right, management, anyone can go
look at who's working on what. Somebody else on my team, oh, look that Rofrano
guy, he's got that one in process, so, um, I’m going to go pick the next one off
the backlog, assign it to myself, and then go work on it. So, some key things to
keep in mind when you're doing your daily execution, nobody should be working on
more than one story at a time.  That's another important feature of having those
little avatars show up because if I see the same avatar, then somebody's working
on multiple stories, and the problem is, I can't ship fifty percent of two
things that are incomplete. I can only ship a hundred percent of one thing
that's completed. So, I don't want people having their focus pulled too many
ways. I want them to work on one thing, deliver a feature, and then go work on
the next feature, unless, of course, they're blocked.  If they're blocked, then
it's okay, while someone's unblocking you, like the scrum master is going to
unblock you, you can start working on a new feature and then get back to the one
that was blocked. When you're finished, you then go create a pull request and
you move that story into review QA. And there's a way to set up pull requests on
GitHub with ZenHub so that when you create a pull request it will automatically
create that pull request in Review QA. And if you assign a story to that pull
request, you sign a Git issue to that pull request, it will pull the issue from
In Process over to Review QA and link them together. So, it's a nice way of
keeping everything neat and tidy so everyone knows a pull request has been made
because now I see things in the Review QA column that I should probably go off
and maybe review for somebody.  And then when the pull request is then merged,
now you can take and drag that into the Done column.  Once your code has been
merged with the base branch, the master branch, or the main branch, you can then
move that to the Done column because you're done.  And then you start all over.
You go back to the sprint backlog, take the next highest thing off the sprint,
assign it to yourself, start working on it.  In this video, you learned that you
need to keep the Kanban board updated so that everyone knows what you're working
on, it's important to always work on the story with the highest priority that
you have the skills for, and working on more than one story at a time may lead
to neither story being finished at the end of the sprint.