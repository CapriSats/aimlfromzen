---
source_url: https://www.youtube.com/watch?v=77OOqXd_97A
source_file: bainbridge_capital-2024-283f2d28-2042-43ad-9a61-874f915f2cab.md
extractor: youtube
fetched_at: 2026-04-26T18:11:48.129134+00:00
char_count: 8910
title: "YouTube video 77OOqXd_97A"
---

[Music]
I have the great pleasure of bringing
back onto the stage Annie
hey hi hi uh thanks for your patience
this is a true Testament of dedication
and determination and how it pays off
and ain't no permissions going to hold
us back
today no no no do you see my screen I do
I'm going to bring it on to the stage
and I'm going to let you have 10 minutes
and I will uh come and see you in 10
minutes see you cool sounds good yeah
and I will I'll try and make this like a
lightning lightning talk so um yeah hi
everyone I'm Annie thanks for your
patience and getting me up here and
thank you to Demetrios um and the mlops
community team for creating this event
and this space it's been so awesome and
even just like the past two talks were
super relevant to um what I'm
doing uh I'm technically a data
scientist but I'm not really sure if I'm
a data scientist anymore I'm kind of
having an identity crisis um with this
crazy world of AI um but yeah I've
worked at really large Enterprises I've
worked for startups and I'm currently
working on building recommendation
systems at private Equity at a private
Equity company and um so I guess I'm
kind of of like a practical application
of of trying to figure out some of the
questions from the last two talks or
last three talks that were just up here
um so yeah I'm speaking to you from the
perspective of someone who like two
years ago I was just a meager data
scientist um training and deploying
regression and tree based models and uh
I'm like that person who is always
running to try and catch the train and I
always feel like I'm late and that's
really been my experience with llms um
but you know we all have to adapt and um
so I've been adapting by signing up for
15 udemy courses on um generative Ai and
then never taking them and then trying
to build an llm app in in a weekend on a
time crunch um so yeah I I'm gonna take
some of my own advice and I'm going to
think from the end of this presentation
which is now in like less than 10
minutes from now and uh I hope that at
the end of this not only do you feel
like a winner but you have some key
questions to think about um when
deploying llms in production whether
that's on your own if you've never done
it before or if your company or
organization is um looking to deploy
llms in
production um and I hope that you kind
of feel a sense of empowerment that you
can get production experience with llms
um if I did so
um as humans like we're not really built
to think from the end and that's what
makes like product managers jobs so hard
right um so uh I'm going to try and do
that with an example that's kind of
loosely based on my experience right now
of preparing to deploy
llms um so maybe a business leader says
I want to I want a user to find a match
within the first five recommendations
that they see in the application um in
my case a lot of our users can be
Boomers so people who might not have
grown up in the tech age they're not
used to using applications so we have
like a really quick minute for them to
either enjoy their experience or not
enjoy their experience um and let's
assume that these recommendations in our
app um are developed using llms so
already with this business need we're
thinking about the user's experience how
good the recommendations are um what
data a new user would need to input to
receive a good recommendation and how
quickly the app can produce a
recommendation Based on data or even new
data so
um in the data science life cycle which
is something that I'm most accustomed to
and kind of like what I grew up on um it
can be somewhat linear and with the end
goal you know being like get good model
performance and you know go back and get
quality data engineer better
features um and so this thinking can be
somewhat linearly and um like even where
I currently work um we're not even at a
stage where we're able to you know
fine-tune llms or or even use rag we're
just using inference um but we have
naturally leaned on llms for new nearly
every step of the data science life
cycle because it's just so convenient
and so useful um we mostly have
unprocessed text Data as our inputs and
we don't currently have labels so um
using llms it's like a given that that
we're going to use it in our data
science life cycle um llms have proven
to be useful for um cleaning up um text
Data that's scraped from the internet uh
engineering features and creating
similarity searches
so um you know getting there and um
getting some recommendations is just one
part of this this business need that we
have um but once we have those good
recommendations and we've sort of been
through that data science life cycle um
if we go back to that business need that
only covers just a small portion of that
business need which is getting good
recommendations um so some of the other
questions that we need to ask if we're
going to have llms anywhere in the life
cycle of our product um so like as an
example we use open AI API as part of
our data cleaning process um there are
rate limits on the API and it's costly
so how long will it take to process data
users at once um doing things like
tokenization and text embeddings that's
different from the realm of like
traditional data science pre-processing
that I've done in in production so like
what is the compute on something like
that um what's the compute on running
pre-trained llms like Bert um going back
to like the evaluation piece like how do
we evaluate this and collect the right
data points to see if the predictions
that our llms are making or the similar
researches that they're doing are um
what we want the user to
experience and then also like
if the similarity search or like the llm
is utilizing like a description for
example of a business or of a person
who's using the application um how do we
collect like quality data from the user
so that we know that it's going to
produce a good
recommendation um you know we can't have
a user come in and just give us a one
sentence description and hope that um
that will be quality enough to have them
have a good experience so how much do we
guide
that and I've watched um data
scientist's eyes glaze over when they
suddenly realize um that the cool
results that they produced using an
llm be reproduced AO like and automated
um in the world of the
app so um I'll just skip ahead here
because um you know like I think
ultimately I I really wanted to give an
example of how you could like simple um
quick and dirty deploy an llm which is
kind of like what I'm trying to do right
now but I realized that like in some
ways it's like not it's not simple and
so like where I'm at is I'm working on
deploying our models in AWS Cloud um no
particular tie to AWS it's just the
cloud service that we use um so that I
can kind of test the limits of all these
questions that I'm asking and
uh and so just as like if whether you're
on your own right now trying to figure
out how to deploy llms or you work for a
company that's interested in deploying
llms um the cool thing is that a lot of
the cloud services especially AWS offer
a lot of Integrations with llms so you
could um create an AWS account if you
don't already have one and use um the
sage maker Integrations with hugging
face to deploy your llms that means like
you don't even have have to download the
model artifacts to deploy an llm um also
AWS
Bedrock allows you to invoke a an llm on
the Bedrock runtime and just yesterday
deep learning AI released a free course
on um creating serverless llm apps with
bedrock so again like this is something
where like you don't need to like get a
job to um then get the experience that
you need to deploy llms you can like go
out and play with some of this stuff
yourself um even if it seems a little
bit scary um or you haven't really
explored this world yet um so yeah and
even if you just tried this you would be
at where I'm at right now so um I guess
in conclusion like um uh you know this
is kind of like deciding to have kids
there's never a right time while you'll
be ready to start deploying llms so um
go play with it and uh
yeah thank
you I love this quote at the end this is
so awesome and I was trying to tweet
what you were saying like I wanted to
give a quick and dirty way of deploying
llms except I realize there's not really
a quick and dirty way of doing this it's
amazing even if the marketing teams want
you to think that there is that's the
problem with it I think huh yes
absolutely absolutely yes if you ask any
marketing team right now they will tell
you that it's easy as you know it's like
that that classic meme where half the
horse is drawn with stick figures and
then the other half is drawn uh yeah
exactly really detailed in depth and so
it's like how to draw a horse and draw
that so Annie awesome thank you so much
for persisting and giving us this talk
it was awesome I really appreciate you
coming on here thank
[Music]
[Applause]
[Music]
you
