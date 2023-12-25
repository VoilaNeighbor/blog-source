In the [last blog](./Setting%20up%20a%20Blog%20Site.md), I set up a very crude
blog site, with just a simple page exported from Notion. Now, I’m adding
essential features so that I could update my blogs without going back to my
Notion draft.

There are endless possibilities for a blog site. For editing, I could introduce
beasts into play such as *editor.js*, *Monaco* and *Code Mirror*. For styling,
I could introduce existing component libraries. For content scripting, I might
set up a backend server, which involves more than domain configuration and
network issues… I still remember that I am learning to take small steps on the
happy path to gain confidence; so no, not those fancy things, at least for now.

The core of the automating the blog posting process is the separation between my
blog source and how it’s presented. To do this, I need a custom compiler. The
compiler should cut short paths tailored for my needs, otherwise it won’t be
any better than off-the-shelf solutions.

Now there are going to be three parts: the compiler, the blog sources, and the
compiled web pages. It is worth it to use Git Submodules to separate the commit
history of each repo, with a small amount of effort.