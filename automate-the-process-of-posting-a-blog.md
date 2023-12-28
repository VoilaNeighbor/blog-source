# Automate the Process of Posting a Blog

In the [last blog](./Setting%20up%20a%20Blog%20Site.md), I set up a very crude
blog site, with just a simple page exported from Notion. Now, I’m adding
essential features so that I could update my blogs without going back to a
Notion draft.

There are endless possibilities for a blog site. For editing, I could introduce
beasts into play such as *editor.js*, *Monaco* or *Code Mirror*. For styling, I
could introduce existing component libraries like *Material UI*. For content
scripting, I might set up a backend server, which involves more than domain
configuration and network issues… I still remember that I am learning to take
small steps on the happy path to gain confidence; so no, not those fancy
things, at least for now.

The core of automating blog posts is the separation between the
blog source and how it’s presented. To do this, I need a custom compiler. The
compiler should cut short paths tailored to my needs, otherwise, it won’t be
any better than off-the-shelf solutions.

![Repo structure](./automate-the-process-of-posting-a-blog.svg)

## A Handmade Prototype as Reference

The other day, I shared this concern to a friend: how do you test drive frontend
development efficiently? We need humans to check if the visuals are correct.

My friend, working at a big tech company, raised her eyebrow: "Nope. It's
actually straight forward. We have specialist UX designers working on
requirement documents, so we always have a concrete criterion to meet."

Something I overlooked before was that analysis and designing are arts of their
own. Even in agile development, a terse design document is still better than
nothing. This applies to personal projects, as well.

For me, the prototyping procedure is as simple as creating a local HTML draft
in the browser and toy with the tags and styles.

## An End-to-end Skeleton

A unit test can never contribute as such confidence as an *acceptance test*, aka
*end-to-end test* (E2E test). Those who claim it's not are just still ignorant of themselves
doing this manually all the time. It should be a shame, as programmers should
be proud of automating repeated labor, instead of getting numb about it. So, I'm
in strong support of E2E test scripts as the first step of the project.

For now, I can think of these points:

1. Pull the latest blog compiler and sources.
2. Run the compiler on the sources to get the latest blog output.
3. Commit and push, which equals to "deployment" with GitHub pages.

Some extra points:

1. A dedicated branch for the releases, e.g., *main*. I think it's dangerous to 
   have a program writing to the same branch with human. Reminds me of the safety
   principle that there needs to be a human in the loop of any critical systems.
2. Should be able to override the branch to test the automation script itself.

```sh
zig run deploy.zig -- \
    --compiler-commit
```

## Rudimentary Implementation of the Markdown-to-HTML Renderer

