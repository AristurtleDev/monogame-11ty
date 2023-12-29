# MonoGame 11ty Site
This project is a proof of concept to present to the MonoGame Foundation as an alternative to building the website using 11ty instead of only DocFx.

Live Preview: https://mgdocs.aristurtle.net

## Motivation
DocFx is a wonderful tool for generating an API documentation site for a .NET project.  However, the usefulness of the tool ends there.  It is not designed to be a general purpose static site generator and instead focuses only on it's strength of being a documentation static site generator.

The MonoGame Foundation is currently using DocFx to generate not only the API and supplementary documentation, but also to generate the static sites for the various pages on their website such as the landing page and about page.  Doing this within DocFX only leads to issue where you either have to design an entire DocFX template from scratch or use CSS hacks to get around some limitations that are placed in the default and modern templates of DocFX.

## Purpose
The purpose of this proof of concept is to show that the website used for MonoGame can still be done from a static site generator that allows the flexibility of designing a proper website while also incorporating the generated documentation from DocFX.  

For example, since DocFX uses Mustache as the templating language, this means it's logic-less.  There are is no way to have the templates generate paginated pages or filters based on the data for those pages.  In 11ty, by default we are using Nunjucks (.njk) templating, which does allow for logic.  This allows the creating of things such as the [Blog](https://mgdocs.aristurtle.net/blog) page in which the foundation can post relavent news on MonoGame and the foundation instead of just listing links in the About page [like is currently done](https://monogame.net/about.html)

## More Information
For additional information on the changes that this proof of concept brings, please visit the [Website Refresh](https://mgdocs.aristurtle.net/blog/2023-12-29-website-refresh/) blog post.

