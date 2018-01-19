# The Biggest Mistakes I See People Make on GitHub

GitHub, as a development model (capably cloned by open-source projects like GitLab and Gitea) and as an open-source development community (irreplaceable), is *spectacularly* powerful. The term "world-changing" [gets thrown around pretty recklessly in tech these days](https://www.youtube.com/watch?v=IXuFrtmOYKg), but I really do believe that Git, and the extension of its facilities through GitHub, has the real, tangible potential to enable a better future.

However, there are a lot of heartbreaking instances where I see that potential being inhibited or outright squandered, so I'm going to illuminate those here, in the hopes that these mistakes may be ameliorated.

To reiterate (because I know the repo name might be misleading), this is a list of common mistakes made by *users* on GitHub. For a list of mistakes made *by* GitHub, check out https://github.com/isaacs/github/issues.

## Not reading the documentation

Okay, so first off: [**you should read the GitHub Guides**](https://guides.github.com/). These cover the most important things about using GitHub, and *most* of the power of GitHub is described in these guides.

There are some topics that those guides do gloss over, though, which is why I created this repo.

## Not discussing ideas in Issues

GitHub Issues are essentially a public forum where anybody with a GitHub account can participate in development discussions. This is *almost always* a good thing, and in the rare case where an issue gets unmanageably dogpiled by bikeshedders who have nothing worthwhile to say (but will say it anyway), you can lock the issue to repository participants.

File issues early, and file issues often. Discussing your idea, whether it's as vague as "This one thing feels a little bit kinda weird", as colossal as "this shouldn't run on electronic devices at all", or as specific as "the getUsersByBirthDate function should return an array of objects instead of an array of strings", it's worth describing initially as a freeform message, even if just as a note for yourself (which you can then *reply* to yourself, which can provide a useful record of how your idea on the subject evolved).

For some idea of how discussions in Issues can be a useful prefigure to committed development, see [the issues on this repo](https://github.com/stuartpb/github-mistakes/issues) for some ideas that haven't been covered in this guide yet.

## Not creating organizations for big projects

If your project is large enough to merit:

- more than one developer
- subsidiary projects / repositories
- its own domain name and/or logo

you should have created an organization for it. [Here are *just a few* of the many reasons why.](https://github.com/stuartpb/how-i-roll/blob/master/starting/apps.md#step-2-create-an-organization-on-github)

It's okay to have not realized this when you were originally creating the project: migrating a repo from your personal account to an org you're a member of is a two-click operation from that repo's settings.

## Not using GitHub Pages whenever possible

If you've got *any* sort of static web content in your repository, you should turn on GitHub Pages to host it. Otherwise, you're just making harder to browse your repo's content for no good reason.

## Leaving things out of repositories

Your project's logo should live (in a vector format, specifically SVG) in a repository in your organization, not in your team's private Dropbox or in the "My Pictures" directory on your art director's home PC. (I mean, it can still live there *too* if you've got it tracked in a repository: that just shouldn't be the *only* place for it). Having it versioned (with commit message metadata) makes it clear who worked on it, when it's been updated, what the update changed (GitHub offers [*three different kinds* of visual diff](https://help.github.com/articles/rendering-and-diffing-images/)!), *why* it was changed, and *anything else an interested party might want to know*.

If your project requires a complicated setup / configuration to build it, that configuration should live alongside the code, with documentation about how to install it. When it comes to continuing your work, code that can't build on anyone else's machine (or *your next* machine) might as well not exist.

## Naming repos like the username / orgname is a prefix

Your username / orgname doesn't move with the repo when someone forks it to their own account (ie. to submit a pull request): if you've got a repo called "foobar/docs", and I go and fork that repo, it would now be called "stuartpb/docs", which makes no sense. If the content in your repository is specific to you as a user/org, you should *repeat your username/orgname as a hyphenated prefix on the repository* (eg. "foobar/foobar-docs"). This is no more redundant than the way the primary project in your org is probably called something like "foobar/foobar" anyway.

Some users have repos like [sindresorhus/ama](https://github.com/sindresorhus/ama), where the repo only contains guidelines about how to work with the project, and the real interaction is in issues: this is *okay*, since issues don't migrate with forks, and the "ama" repository content can reasonably map onto a new user who forks it (and be customized to apply back to them accordingly). However, if the *vast majority* of the content in the repository is specific to you (ie. if somebody forking your repository would most likely be doing so with the intent of *contributing a patch for **your** content*), you should prefix it with your name.

## Using capitalization (or underscores) in org/user/repo names

This is a minor thing, but if your organization's name and/or its projects are capitalized, it bucks the convention followed by the *vast* majority of users, projects, and orgs on GitHub, and it signifies you as a clueless outsider to the community at large [*(cough cough Microsoft cough)*](https://github.com/Microsoft).

There are *times* that you may want to use underscore instead of hyphens or capitalize a repo name (ie. to publish a package in an ecosystem where modules are generally capitalized), but if you do it *normally*, it has the same disquieting feeling as coming acros a project where a lot of the core filenames contain spaces. (If you don't understand what's disquieting about that, go ask a developer whose role involves using a command line.)

## Making developers create a "company account"

I've seen some companies request that their employees participate in the company's development on GitHub using a fresh account, distinct from their personal account, that will only be used to develop things for that company.

This is weird and possessive, and it's a *major* turnoff for any high-profile maintainers you might want to hire for their work on an existing project. Capitalizing the org name might make your company's GitHub activity *smell*, like a fart in an elevator: dismembering your developers' professional lives will make it *stink like a pile of corpses*. The only developers who won't feel straitjacketed by this are ones who've had no contact with the open-source world, either because they're fresh-faced out of Junior Dev School, or because they've been trapped behind a pile of binders writing COBOL for forty years.
