[![Build Status](https://travis-ci.com/carpentries/workshop-template.svg?branch=gh-pages)](https://travis-ci.com/carpentries/workshop-template)

# UCSB Fall 2021 SQL data Carpentry

This repository was made from The Carpentries' ([Software Carpentry][swc-site], [Data Carpentry][dc-site], and
[Library Carpentry][lc-site]'s) template for creating websites for workshops.



Please *do your work in your repository's `gh-pages` branch*, since that is what is
   [automatically published as a website by GitHub][github-project-pages].

Once you are done, please also [let us know][email] the workshop URL. If this is a self-organised
   workshop, you should also [fill in the self-organized workshop
   form][self-organized-workshop-form] (if you have not already done so), so we can keep track of
   all workshops. We build the list of workshops on our websites from the data included in your
   `index.md` page. We can only do that if you [customize][customization] that page correctly *and*
   let us know the workshop URL.

If you run into problems,
or have ideas about how to make this process simpler,
please [get in touch](#getting-and-giving-help).
The pages on [customizing your website][customization],
the [FAQ][faq],
and the [design notes][design] have more detail on what we do and why.
And please note:
if you are teaching Git,
please [create a separate repository](#setting-up-a-separate-repository-for-learners)
for your learners to practice in.

## Video Tutorial

There is a [YouTube video](https://www.youtube.com/watch?v=_Ag1JiZzyUQ) that demonstrates how to
create a workshop website.




4.  Remove the notice about using the workshop template in the `index.md` file. You can safely
    delete everything between the `{% comment %}` and `{% endcomment %}` (included) as indicated
    below (about from line 35 to line 51):

    ```jekyll
    {% comment %} <------------ remove from this line
    8< ============= For a workshop delete from here =============
    For a workshop please delete the following block until the next dashed-line
    {% endcomment %}

    <div class="alert alert-danger">
      ....
    </div>

    {% comment %}
     8< ============================= until here ==================
    {% endcomment %} <--------- until this line
    ```



### Update the content of the README file

You can change the `README.md` file in your website's repository, which contains these instructions,
so that it contains a short description of your workshop and a link to the workshop website.


## Additional Notes

**Note:**
please do all of your work in your repository's `gh-pages` branch,
since [GitHub automatically publishes that as a website][github-project-pages].

**Note:**
this template includes some files and directories that most workshops do not need,
but which provide a standard place to put extra content if desired.
See the [design notes][design] for more information about these.

Further instructions are available in [the customization instructions][customization].
This [FAQ][faq] includes a few extra tips (additions are always welcome)
and these notes on [the background and design][design] of this template may help as well.


## Creating Extra Pages

In rare cases,
you may want to add extra pages to your workshop website.
You can do this by putting either Markdown or HTML pages in the website's root directory
and styling them according to the instructions give in
[the lesson template][lesson-example].


## Installing Software

If you want to set up Jekyll so that you can preview changes on your own machine before pushing them
to GitHub, you must install the software described in the lesson example [setup
instructions](https://carpentries.github.io/lesson-example/setup.html#jekyll-setup-for-lesson-development).

## Setting Up a Separate Repository for Learners

If you are teaching Git,
you should create a separate repository for learners to use in that lesson.
You should not have them use the workshop website repository because:

* your workshop website repository contains many files that most learners don't need to see during
  the lesson, and

* you probably don't want to accidentally merge a damaging pull request from a novice Git user into
  your workshop's website while you are using it to teach.

You can call this repository whatever you like, and add whatever content you need to it.

## Getting and Giving Help

We are committed to offering a pleasant setup experience for our learners and organizers.
If you find bugs in our instructions,
or would like to suggest improvements,
please [file an issue][issues]
or [mail us][email].

[email]: mailto:team@carpentries.org
[customization]: https://carpentries.github.io/workshop-template/customization/index.html
[dc-site]: https://datacarpentry.org
[design]: https://carpentries.github.io/workshop-template/design/index.html
[faq]: https://carpentries.github.io/workshop-template/faq/index.html
[github-project-pages]: https://help.github.com/en/github/working-with-github-pages/creating-a-github-pages-site
[issues]: https://github.com/carpentries/workshop-template/issues
[lesson-example]: https://carpentries.github.io/lesson-example/
[self-organized-workshop-form]: https://amy.carpentries.org/forms/self-organised/
[swc-site]: https://software-carpentry.org
[lc-site]: https://librarycarpentry.org
