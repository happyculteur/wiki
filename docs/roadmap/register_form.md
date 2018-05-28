# Register form

The first step is to get a database of people who will be using our platform,
so it doesn't go live empty.<br>
To do so, we need a register form, right now running not open source on
[this page](https://join.happyculteur.co).

The idea is to bypass this form since our dev community is pretty small and
doesn't master the technologies involved in this form (VueJS + GraphQL).<br>

To make it simple, we want to generate a simple static page, explaining the
purpose of our data collection (#RGPD) and right after this explaination, a
link to a [TypeForm](https://www.typeform.com/) or [Google Form](https://www.google.com/forms/about/).

So the steps are the following:

  * [ ] Creating the form on Google or TypeForm
  * [ ] Generate the static page (no matter the techno, [Hugo](https://gohugo.io/) or whatever.
  * [ ] Publish the static page on S3 with an automated pipeline (yes we love automation!)
  * [ ] Communicate onto the form release
