---
layout: post
title: Why most mobile apps suck or 'What mobile web devs can learn from game devs'
categories:
- technology
status: publish
type: post
published: true
comments: true
meta:
  _edit_last: "1"
  dsq_thread_id: "781326410"
---
<em>Thanks for all the attention this post got on reddit! You guys rock! That's some 6,584 rocking people :) <a href="http://www.reddit.com/r/programming/comments/x9c8m/why_most_mobile_apps_suck_or_what_mobile_web_devs/">Join the discussion</a>.</em>

I've been arguing recently with a few folks that the reason Facebook mobile apps suck isn't because they chose HTML5 blend over pure native but rather due to poor execution on their side.

There were a bunch of articles written to support both sides but arguing about it isn't really productive, is it? Last night I read an amazing article by <a title="Patrick Wyatt" href="http://www.codeofhonor.com/blog/author/patrick-wyatt">Patrick Wyatt</a> – <a title="The making of Warcraft part 1" href="http://www.codeofhonor.com/blog/the-making-of-warcraft-part-1" rel="bookmark">The making of Warcraft part 1</a>. I hope you played Warcraft or at least Warcraft 2.

The problems outlined there make our today's hurtles laughable. Fitting a game into 640Kb of memory, code versioning via "remembering which files are changed on that floppy disk", huge multiplayer latencies.

We are spoiled these days and some of us got too comfy thinking 3G and LTE can solve all those latency problems for you. The real answer to the problems with most mobile apps these days (including Facebook's) is Patrick's another great article – <a title="Reducing perceived latency" href="http://www.codeofhonor.com/blog/reducing-perceived-latency" rel="bookmark">Reducing perceived latency</a> and Mike Krieger's (Instagram) – <a href="https://speakerdeck.com/u/mikeyk/p/secrets-to-lightning-fast-mobile-design?slide=1">Secrets to Lightning Fast Mobile Design</a> slide deck.

Slide 25 sums it up nicely in three 'easy' steps:

1. perform actions optimistically
2. adaptively pre-load content
3. move bits when no-one's watching

The later two are pretty self-explanatory, but I'd like to elaborate a bit more on the first one. First time I saw it I assumed it ment optimizations, but what it really means is optimism.

Be optimistic about the and make the user feel productive. Here's one of the slides:
<p style="text-align: center;"><img class="aligncenter  wp-image-318" title="Secrets to Lightning Fast Mobile Design – Slide 34" src="http://dybskiy.com/wp-content/uploads/2012/07/Instagram-slide-34.png" alt="" width="789" height="760" /></p>
Just like Ogre in Warcraft would say “Daboo” once you command to move, it didn't really mean that all the requests had finished. It was a simple acknowledgment for the user that we got your command.

What if the request fails? Notify user unobtrusively:
<p style="text-align: center;"><img class="aligncenter  wp-image-320" title="Slide 38" src="http://dybskiy.com/wp-content/uploads/2012/07/Slide-38.png" alt="" width="272" height="381" /></p>
At the end of the day, choosing tools you use is important but much more important is how you use them.

In light of some Vancouver game studios shutting down I don't think people need to be worried – it could be great for many companies if a game dev joined them.

So if you are a dev looking for work in Vancouver – get in touch with <a href="http://twitter.com/bmann/">Boris Mann</a> or <a href="http://twitter.com/igorskee/">Igor Faletski</a>. They helped me find <a href="https://twitter.com/unbounce">Unbounce</a> team and I can't recommend them enough.

If you read this far, follow me on twitter – <a href="http://twitter.com/dybskiy/">@dybskiy</a>

Thanks to sidcool1234 for submitting to <a href="http://www.reddit.com/r/programming/comments/x9c8m/why_most_mobile_apps_suck_or_what_mobile_web_devs/">reddit</a>.

<strong>Update 1:</strong> reddit reader <a href="http://www.reddit.com/user/barsoap">barsoap</a> pointed out the following:
<blockquote>There's one keyword here: <em>Immersion</em>.

Immersion breakers kill every game, and while break of workflow might not kill an application, it's definitely going to make it suck.

The difference in game vs. app developers here is that game developers focus on immersion from the get-go, even design their games around it, while app developers start off with a set of functionality and, at least hopefully, consider immersion as an afterthought.

Do you remember Kai Krause's early work, such as Kai's Photo Soap? Those were designed around immersion, not functionality.</blockquote>