# The Biggest Mistakes I See People Make on GitHub

GitHub, as a development model (capably cloned by open-source projects like GitLab and Gitea) and as an open-source development community (irreplaceable), is *spectacularly* powerful. The term "world-changing" [gets thrown around pretty recklessly in tech these days](https://www.youtube.com/watch?v=IXuFrtmOYKg), but I really do believe that Git, and the extension of its facilities through GitHub, has the real, tangible potential to enable a better future.

However, there are a lot of heartbreaking instances where I see that potential being inhibited or outright squandered, so I'm going to illuminate those here, in the hopes that these mistakes may be ameliorated.

## Not reading the documentation

Okay, so first off: [**you should read the GitHub Guides**](https://guides.github.com/). These cover the most important things about using GitHub, and *most* of the power of GitHub is described in these guides.

There are some topics that those guides do gloss over, though, which is why I created this repo.

## Not discussing ideas in Issues

GitHub Issues are essentially a public forum where anybody with a GitHub account can participate in development discussions. This is *almost always* a good thing, and in the rare case where an issue gets unmanageably dogpiled by bikeshedders who have nothing worthwhile to say (but will say it anyway), you can lock the issue to repository participants.

See [the issues on this repo](https://github.com/stuartpb/github-best-practices/issues) for topics that aren't yet covered.

## Not creating organizations for big projects

If your project is large enough to merit:

- more than one developer
- subsidiary projects / repositories
- its own domain name and/or logo

you should have created an organization for it.

It's okay to have not realized this when you were originally creating the project: migrating a repo from your personal account to an org you're a member of is a two-click operation from that repo's settings.

## Not using GitHub Pages whenever possible

If you've got *any* sort of static web content in your repository, you should turn on GitHub Pages to host it. Otherwise, you're just making harder to browse your repo's content for no good reason.

## Naming repos like the username / orgname is a prefix

Your username / orgname doesn't move with the repo when someone forks it to their own account (ie. to submit a pull request): if you've got a repo called "foobarcorp/docs", and I go and fork that repo, it would now be called "stuartpb/docs", which makes no sense.
