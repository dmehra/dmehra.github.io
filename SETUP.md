# How to run a newsletter

* TOC
{:toc}

## With GitHub Pages and Mailchimp

This is the easiest setup I could think of. I keep my signup page for the Tester's Digest newsletter in the index file of my [GitHub Pages](https://pages.github.com/) site. The archive of past issues is also kept there, with each issue written and committed as a [Markdown](https://guides.github.com/features/mastering-markdown/) file. GitHub Pages is free for public projects. This gives me revision control, no worries about backing up content, high availability, and ease of authoring in Markdown.

Distribution of the newsletter is handled via [Mailchimp](https://mailchimp.com/) service, which is also free up to a certain number of subscribers, which this little newsletter would be lucky to ever reach. The Mailchimp signup link is pasted into the index page; unsubscribes and anti-bot defenses are handled by Mailchimp so I don't need to worry about any of that.

When I compose a new issue of the newsletter, I add a new markdown file to the archive, and link it off the archive index page. Then I create a new "campaign" inside Mailchimp account, paste the markdown as is into the body of the email, and push the big red button. Done!

## Publishing a new issue

Make a file for the new issue (I usually copy off an old one):

```
cp archive/testers_digest_2017_03_05.md archive/testers_digest_2017_03_12.md
```

Edit the file, be sure to change the issue number and date, then supply new contents.

I keep two main sections: "Topic: XYZ" and "Off-Topic" for others news that caught my eye.

Link the new issue from the archive index by editing [](archive/index.md) file.

To view the markdown pages locally with proper rendering, [run local Jekyll](https://help.github.com/articles/setting-up-your-github-pages-site-locally-with-jekyll/):

```
$ bundle exec jekyll serve
```

Then access the local copy of the site at [port 4000](http://127.0.0.1:4000/). Note that good old [grip](https://github.com/joeyespo/grip) doesn't render GitHub flavored markdown quite right, so the above approach is preferred. The setup to make it work was simply to make a [Gemfile](Gemfile) with the right incantation, then run `bundle install`, that's it.

Commit the changes:

```
git add archive/testers_digest_2017_03_12.md
git add archive/index.md
git commit -m "Adding issue #6, topic: continuous testing"
git push
```

Wait a bit, up to a few minutes (GitHub Pages has pretty slow caching), then validate in place on [Tester's Digest site](http://testersdigest.mehras.net/archive/).

Just in case, I click each link to make sure I didn't mess up. Nobody wants broken links in their newsletter.

## Distributing a new issue

To mail out the newsletter to subscribers, I go to my [Mailchimp account](https://login.mailchimp.com/), click Campaigns, then "Create Campaign".

* Campaign name = "Newsletter #X"
* Campaign type = "Plain-text"
* Click "Create" button.

Then click through using "Next" button that's hiding in the lower right corner, keeping the defaults:

* Keep "Entire list" setting
* (click Next)
* At Campaign Info screen, enter Email subject = "Tester's Digest #X"
* Keep "Track plain-text clicks" setting under Tracking
* (click Next)

Get to the step of actually putting together the newsletter email:

* Copy-and-paste markdown contents of the issue into the left window pane
* (click Next)

Send it out:

* Click "Send" button in lower-right
* Push the big red "Send Now" button, very satisfying
* Check my own inbox since of course I have a subscriber test account

## FAQ

### Why are you doing this?

The newsletter? Simply because I read a lot, and I figured, some of the things I read may be useful to share with others in the software testing field. I have no further agenda.

### What is the newsletter frequency?

Weekly-ish. I try to publish every Sunday.

### Is there an RSS feed?

Yes, there is an Atom feed. I set it up using [jekyll-feed plugin](https://help.github.com/articles/atom-rss-feeds-for-github-pages/).

### Why do Tester's Digest emails have `<angle brackets around the URLs>` ?

Due to a quirk of GFM (GitHub Flavored Markdown), I have to put the URLs inside angle brackets when writing the markdown files. They render fine on the GH Pages site, but the brackets show up in newsletter emails. There is no way around this, short of hand-editing the brackets out of the markdown when creating a Mailchimp campaign. That would be error prone, and I cannot be bothered. The angle brackets stay.

### Is there any click tracking due to using Mailchimp?

Nope. Because I pick plain-text campaign type in Mailchimp, and only leave the required "Track plain-text clicks" setting enabled, the sole tracked link is the Unsubscribe one at the bottom of the email. The links to articles/posts in the newsletter have no tracking on them.

Moreover, I make sure I remove any fields after `?` in the URLs before including them into the newsletter, so I don't pass on the tracking that may have been included by original publisher.

I don't often wear a hat, but when I do, it's tinfoil.

This has a side effect of not knowing if my subscribers ever read anything I send out. I can live with the mystery.

### How does testersdigest.mehras.net redirect to GitHub Pages?

Via a CNAME record from my web hosting provider that makes my subdomain [testersdigest.mehras.net](http://testersdigest.mehras.net) point to my GH Pages site [dmehra.github.io](http://github.com/dmehra/dmehra.github.io).

To set this up, I used these excellent [instructions](https://github.com/tomkeays/cname-setup) because GitHub's own [doc](https://help.github.com/articles/using-a-custom-domain-with-github-pages/) was a bit opaque.

### Any other customizations that were needed?

GH Pages use [Jekyll](https://jekyllrb.com/docs/github-pages/) as the static site generator. There are built-in themes you can use to make the site look decent. I went with [Dinky](https://github.com/pages-themes/dinky) so that's in my `_config.yml` file.

The default Dinky was creating duplicate "View on GitHub" buttons on my index page, so I copied off `_layouts/default.html` and commented out the extra button. I also added the EFF badge image in the footer.

I added a `favicon.ico` PNG file to get that "TD" marker in the browser tab or bookmark. I made the image myself by using Google's free font library.

The index page for the site is in Markdown because why not, Jekyll transforms it into index.html. It includes the embedded signup form snippet provided by Mailchimp. The form "just works".

### How to get SEO and Slack URL unfurling for posts

I noticed that links to Tester's Digest issues were not getting a nice little snippet when posted in Slack. Quick investigation showed that this fanciness, called [URL unfurling](https://medium.com/slack-developer-blog/everything-you-ever-wanted-to-know-about-unfurling-but-were-afraid-to-ask-or-how-to-make-your-e64b4bb9254), is based on SEO (Search Engine Optimization) metadata which I didn't have, hence this newsletter was also not enjoying SEO benefits. Here is how I [added metadata tags with Jekyll](https://github.com/jekyll/jekyll-seo-tag#usage) and Markdown:

Added to `Gemfile`:

```
gem 'jekyll-seo-tag'
```

Added to `_config.yml`:

```
gems:
  - jekyll-seo-tag
```

Added right before `</head>` in the site template `_layouts/default.html` (without the extra spaces):

```
{ % seo % }
```

Then in markdown of each post, I added "front matter" section that is transformed by Jekyll into the meta tags when generating html page:

```
---
description: What this post is about.
---
```

Note a gotcha that colon character `:` is not welcome inside the description.

I tried overriding `title` in the markdown front matter, but it wasn't getting picked up, so I stayed with the default site-wide title "Tester's Digest". I also tried adding image tag to get a thumbnail logo for the unfurled URLs in slack, that didn't work either, sticking with the "good enough" solution of description metadata.

Here is what comes out in HTML:

```
{% seo %}
```
