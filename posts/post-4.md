---
title: "Problems with AI web development"
url: "https://allister-myth.netlify.app/posts/post-4"
description: "A casual blog about where I post anything I am working on or find interesting.
"
---

[Back to Home](/)

![Problems with AI web development](/_astro/web.pfN5J4uD_27aKC2.webp)

# Problems with AI web development

*   *   [Machine Intelligence](/categories/machine-intelligence)
    |
*   25 May, 2026 |
*   02 Mins read

I wanted to make a portfolio website a few days back and made the mistake of relying on AI. I had made a website before but thanks to every top result shown on google, I got convinced that making my site with AI was a good idea.

So I started simple, went on Claude and asked it to make a site. All good; the website is ready and looks okay but needs something more. So I spend the next few minutes customising the site with Claude of course. The site looks sleek and I feel great. Then I thought why not make a blog page (this one didn’t exist back then) and that was the beginning of the end. It did make a blog page, nice and good looking. The only issue was that the blogs were hardcoded in the code so every time I had to write a blog I would need to update the main code of the blog which as you probably guessed would become huge in just a few days. So I asked it to make a dynamic blog and it suggested to use react for that. Down goes the whole thing as I begin to start generating the whole code again with react and fine tuning it.

Eventually I did make the whole site again. I ran it on localhost and everything worked great. So I pushed it on a Github repo. White screen…. Nothing. Back to AI to try and debug it. Apparently some router issue for the blog page. The AI suggests a fix, I do it. Now even the localhost is dead. Asked the AI to fix it, it tells me a single page is enough for my site, I shouldn’t have made a blog page which it told me was a great idea at start. So I slowly try to debug it using different AIs. A few hours wasted on this and I realise the biggest issue, the AI itself. Whenever I made a request to debug, say X feature is not working sometimes instead of correcting the X feature, it would try to delete the X feature or change its code so it looks good on surface but doesn’t work properly which would cause even more debugging problems. I was getting frustrated and became adamant on fixing the site. But the site was cooked, the main code stopped making sense to me as yet another beautiful feature of AI writing is how it doesn’t follow normal code writing style and uses obscure functions. All the main code…. Delete.

Third time’s the charm ey. So I start writing the code the third time. This time mainly by myself just asking basic questions regarding react from AI. I used Astro for the blog site and it took me a few hours but finally made the site with clean code and a good blog site. By the end, the time it took for me to make the site myself was less than the time I used AI. I now understand why developers dislike AI. For complex tasks, if used without careful guardrails, it creates more issues than solutions. Learning and doing stuff yourself is more fun anyways instead of idly looking at your screen hoping that AI will fix things.

Allister Myth

## Related Posts

*   [Mathematics](/categories/mathematics)
*   [BioMaths](/categories/biomaths)
*   [Machine Intelligence](</categories/machine intelligence>)

23 May, 2026

## [My First post](/posts/post-2)

[Continue Reading](/posts/post-2)

*   [BioMaths](/categories/biomaths)
*   [Machine Intelligence](</categories/machine intelligence>)

24 May, 2026

## [I made a Cancer Prediction model](/posts/post-3)

[Continue Reading](/posts/post-3)