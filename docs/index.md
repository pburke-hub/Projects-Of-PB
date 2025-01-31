---
title: Home
layout: home
---

My plan for this page (i.e. pburke-hub.github.io/Projects-Of-PB/ ) is to simply have this whole Github Pages website simply direct the user to my other projects' own Github Pages websites.

Hope it works!

Maybe it'll just be links in collapsible boxes (no intro paragraph).

Various attempts:

<!-- I give up on gh-pages relative references!!!
<img src="../../docs/assets/images/F01/07_Output_Tbl-520w.jpg" width="520px" height="77px" loading="lazy" > 

<img src=../../docs/assets/images/F01/07_Output_Tbl-520w.jpg width="520px" height="77px" loading="lazy" >

<img src="/../../docs/assets/images/F01/07_Output_Tbl-520w.jpg" width="520px" height="77px" loading="lazy" >
-->

Testing Div with markdown="1":

<!-- style="overflow-x:auto;white-space:nowrap" markdown="1" -->

<!-- `{: aspect-ratio=520/77}` doesn't work for an image, ergo, try: {: style="aspect-ratio:520/77;"}. DON'T set the div's aspect ratio, then if viewport gets less than 520 wide, the height gets lower than 77! In fact, I see no reason for <div> to have its height or width specified either! 
Also, going to see how/whether align-content CSS property is good for the <>div's when screen is large / wide. If so, then should add it to the "scrolling-div-class". -->

<div markdown="1" class="scrolling-div-class" style="align-content:center" >

![Test Image](https://raw.githubusercontent.com/pburke-hub/Projects-Of-PB/main/docs/assets/images/07_Output_Tbl-520w.jpg){: .img-noloadingppty width="520px" height="77px" style="aspect-ratio:520/77;" }

</div> 

2nd Test of <Div> with markdown="1":

<div style="overflow-x:auto;white-space:nowrap" markdown="1" width="520" height="77">

![Test Image](https://raw.githubusercontent.com/pburke-hub/Projects-Of-PB/main/docs/assets/images/07_Output_Tbl-520w.jpg)

</div> 


Test image:

<div style="overflow-x:auto;white-space:nowrap" >

<!-- ![Test Image](../../docs/assets/images/F01/07_Output_Tbl-520w.jpg)
{: width="520px" } -->

<img src="../../docs/assets/images/F01/07_Output_Tbl-520w.jpg" width="520px" height="77px" loading="lazy" >

</div> 

2nd Test Image:

<!-- ![Test Image](/../../docs/assets/images/F01/07_Output_Tbl-520w.jpg) -->

<img src="/../docs/assets/images/F01/07_Output_Tbl-520w.jpg">

3rd Test Image:

![Test Image](https://raw.githubusercontent.com/pburke-hub/Projects-Of-PB/main/docs/assets/images/07_Output_Tbl-520w.jpg)

4th Test Image:

<div style="overflow-x:auto;white-space:nowrap" >

<!-- ![Test Image](https://raw.githubusercontent.com/pburke-hub/Projects-Of-PB/main/docs/assets/images/07_Output_Tbl-520w.jpg) -->

<img src="https://raw.githubusercontent.com/pburke-hub/Projects-Of-PB/main/docs/assets/images/07_Output_Tbl-520w.jpg" 
  width="520px" height="77px" loading="lazy" >

</div> 

5th Test Image:

<div style="overflow-x:auto;white-space:nowrap" >

<img src="https://raw.githubusercontent.com/pburke-hub/Projects-Of-PB/main/docs/assets/images/07_Output_Tbl-520w.jpg" >{: width="520" }

</div> 

This is a *bare-minimum* template to create a Jekyll site that uses the [Just the Docs] theme. You can easily set the created site to be published on [GitHub Pages] – the [README] file explains how to do that, along with other details.

If [Jekyll] is installed on your computer, you can also build and preview the created site *locally*. This lets you test changes before committing them, and avoids waiting for GitHub Pages.[^1] And you will be able to deploy your local build to a different platform than GitHub Pages.

More specifically, the created site:

- uses a gem-based approach, i.e. uses a `Gemfile` and loads the `just-the-docs` gem
- uses the [GitHub Pages / Actions workflow] to build and publish the site on GitHub Pages

Other than that, you're free to customize sites that you create with this template, however you like. You can easily change the versions of `just-the-docs` and Jekyll it uses, as well as adding further plugins.

[Browse our documentation][Just the Docs] to learn more about how to use this theme.

To get started with creating a site, simply:

1. click "[use this template]" to create a GitHub repository
2. go to Settings > Pages > Build and deployment > Source, and select GitHub Actions

If you want to maintain your docs in the `docs` directory of an existing project repo, see [Hosting your docs from an existing project repo](https://github.com/just-the-docs/just-the-docs-template/blob/main/README.md#hosting-your-docs-from-an-existing-project-repo) in the template README.

----

[^1]: [It can take up to 10 minutes for changes to your site to publish after you push the changes to GitHub](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/creating-a-github-pages-site-with-jekyll#creating-your-site).

[Just the Docs]: https://just-the-docs.github.io/just-the-docs/
[GitHub Pages]: https://docs.github.com/en/pages
[README]: https://github.com/just-the-docs/just-the-docs-template/blob/main/README.md
[Jekyll]: https://jekyllrb.com
[GitHub Pages / Actions workflow]: https://github.blog/changelog/2022-07-27-github-pages-custom-github-actions-workflows-beta/
[use this template]: https://github.com/just-the-docs/just-the-docs-template/generate
