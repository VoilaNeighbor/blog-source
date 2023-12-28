## A Helpless Programmer Saving Himself

I’m an impetuous programmer, haunted by the urge to rewrite everything, and thus
making little progress over time. The other day, I got a serious DDL in sight,
but feeling myself falling into the same trap again. I got so panicked about
botching the serious task that I couldn’t make any moves but stare at the
screen. Then, I tried writing some soothing words to myself on a notebook. I
jotted down a few points that I was unsatisfied with. Now the vague feeling had
been cast down, I started to calm. It is since then that I have realized how
writing something down helps you organize your mind and think more rationally.

I’m also a forgetful programmer. I learn quite a few things, but I cannot
remember every problem I solved. Every once in a while I’m confronted with the
same problem I solved before. This is also where I found recording something was
so useful.

I’ve been keeping notes on paper and on electrons for a while, but I have still
not become a great engineer. My notes are still unorganized, if I ever tried to
organize, and I still get digressed so often that has become a severe penalty on
my efficiency both at work and at personal projects. It was not until I wrote my
end-year self-assessment report that I found that you needed something to show
up your sleeves. One can have thousands of dreams and intentions, but what
matters are the products we materialize. So, I asked myself: why not set up a
blog site if you want to improve your WEB skills? Why not post gamedev series if
you want to get your indie games done? Of course, you do not have enough time to
record every idea, so it’s a selective procedure that forces me to take the most
important pieces.

And thus I got happy and full of motion, and it marks the commence of my blog
site.

## A Wishlist to Taste the Sweetness in One Day

As you might’ve guessed, I’m also haunted by micro-optimization. Yet, in my
failed pursuits of perfection, I’ve learned a key point maybe no one has told
you: emotions matter. We really cannot stick to the most rational path if we
don’t get anything in return for a long time. I’ve given up plans more than I
could remember. What still lingers is the haunting fear of another failure.
Trying to get it done without allowing for dirty points and you will become like
me. In this case, the blog site, my first reaction was to build everything
barehanded as I dream of. But finally, I managed to resist the urge.

I start with writing down things I’d like to enjoy. I cannot enjoy multiple
points at the same time or it’s going to be a mess, so this list helps me
prioritize and sacrifice the lesser points in the bootstrap stage. Here’s what I
want:

- Showing off my “great” blogs to the world.
    - Also, it’s something concrete to show to my family, my friends and the
      future myself that I’m not wasting time day-dreaming, and really doing
      something.
- Set up a discussion panel for readers. I like making friends.
- CSS styling stuff. I like beauty.
    - Also responsive, at least for both landscape and portrait.
- Simplicity & performance maniac. I’m in belief that simplicity in execution is
  proportional to simplicity in the code structure, in the large scale.
- Customized markdown-to-HTML renderer.
    - It’s going to be fun and small-scale to implement a subset.
- Auditable blog changes, which encourages me to improve my blogs over time
  while keeping track of its history.
- Also there are some other projects I’d like to develop, and share my
  experience on the site, but that is out of the scope of this blog.

The wishlist is building up my confidence, because I know in my heart that I
won’t forget the good hopes even if I deviate to dirtier but quicker solutions
for the top points.

## A Plan to Ship My “Great” Blogs to the World

If only considering content delivery, a static site will suffice. But I’m also
going to explore more possibilities of frontend tech, so I shouldn’t limit
myself to tailored blog tools such as Jekyll.

- I’ll stick to personal sites, because
    - Blog platforms are too limiting, yet I’m not content with just writing
      things alone.
    - Blog platforms could monetize on you. (Ref: [Enshittification](https://en.wikipedia.org/wiki/Enshittification))
    - Blog platforms might even try to take the patent of your work and forbid its availability on the Internet.
- I’ll start with GitHub pages so I don’t have to cope with DNS or frontend
  servers.
- Since for the 1st stage, it is only going to be a simple text site, there is
  no need to introduce React and its friends, although I’m very familiar with
  them.

Now that I’ve created a simple GitHub Pages repo, and printed Hello world, I
wanted to port this page, which was originally written on Notion, to my blog
site. This is a nice shortcut, because the styling of Notion exports can be a
good default start.

Modify the content of *index.html* to this:

```html
<ul>
  <li>
    <a href="./Setting up a Blog Site.html">Setting up a Blog Site</a>
  </li>
</ul>
```

Once the changes are pushed to GitHub, I could start to visit the page via the
hyperlink. Doesn’t take me too much time to arrive here! My first though was to
write a Zig script to remove the garbage spit by Notion export, but soon I
realized that my goal was just to set up an available blog somewhere on the WEB,
so I put off the idea. Thanks to the wish list, I won’t be worried that I would
forget the funny things I wanted to do. Similar to the *Single Responsibility
Principle*, I’m trying a *Single Aim Principle* (SAP) for any of my progress.
BTW, I found that “to-do list” sounded negative to me, hence I’ll use the term
“wish list” hereafter.

## Retro

It’s far from finished, but I have already enjoyed it and remembered a great
lesson. The me myself three months ago would definitely go heads straight,
touching every fancy feature I could dream of, and give up because my hands are
too small to hold all the big wishes. As I grow into a more experienced
engineer, I am learning step by step, to eat my meal piece by piece.

It takes confidence to do so. I was eager to prove myself, and turned out to
always be running in the opposite way from success. Now I’m brave enough to
admit that I cannot hold them all, so I resort to existing tools such as GitHub
Pages to simplify the releasing procedure to a minimum, and utilized Notion, the
tool at hand, which I’m writing this blog with, to export a static page. I’m
getting rid of the eagerness to fix the “garbage” in Notion exports, and
learning in return to follow a bigger picture. Somewhere in my heart I believe
firmly that this is still in the vibe of geeks. I’m just learning how to walk
farther without exhausting my will.

```html
<ul id="d8d29e74-2850-4740-8795-a6437335ad70" class="bulleted-list">
  <li style="list-style-type:circle">Blog platforms could monetize on you.
    <figure id="af08cb91-4b45-4bbe-a039-cc97582bfe76">
      <a href="https://en.wikipedia.org/wiki/Enshittification" class="bookmark source">
        <div class="bookmark-info">
          <div class="bookmark-text">
            <div class="bookmark-title">Enshittification</div>
            <div class="bookmark-description">Enshittification, also known as platform
              decay,&amp;#91;1&amp;#93; is the pattern of decreasing quality of online platforms that act
              as two-sided markets. Enshittification can be seen as a form of
              rent-seeking.&amp;#91;2&amp;#93; Examples of alleged enshittification have included Amazon,
              Bandcamp, Facebook, Google Search, Quora, Reddit, and Twitter.</div>
          </div>
          <div class="bookmark-href">
            <img src="https://en.wikipedia.org/static/apple-touch/wikipedia.png"
              class="icon bookmark-icon">https://en.wikipedia.org/wiki/Enshittification
          </div>
        </div>
      </a>
    </figure>
  </li>
</ul>
```

So it really pays off. From the Notion export page, I learned about how they
used CSS, such as *::marker* selectors. I learned about the \<figure> HTML
element. I dreamed a bit about fancy use cases of assigning a UUID to every note
block. My imagination and exploration into an existing piece of work helped me
learn ten times faster than poking around myself with crude tutorials.

I can’t help thinking about an item in the *Zig Zen* as well:

> Avoid local maximums.

So here I’m ending this blog with the quote, with my best regards to everyone
who are willing to learn the hardest as they can and contribute to the realm of
software engineering. Good luck to you and me!