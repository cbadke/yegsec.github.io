This site is built using the [Nikola static site generator](https://www.getnikola.com)
Nikola is a relatively easy system to use. You can read the docs but here's the crash
course.

# Setup Dev Env
Install the tools in the [getting started guide](https://www.getnikola.com/getting-start.html).

Start up nikola environment
```
source &lt;your nikola install dir&gt;/bin/activate
```

Start the Nikola server:
```
nikola auto
```

Once the Nikola server is running you should be able to open [http://127.0.0.1:8000](http://127.0.0.1:8000)
and see the site. Any changes you make to pages, posts, templates or styles will automatically
recompile and reload this browser giving very fast feedback.

# Where are things

Editting the site:

|Page|Files|
|----|-----|
|Front Page|`./themes/yegsec/templates/index.tmpl`|
|Resources|`./pages/resources.md`|
|Schedule|`./pages/schedule.md` and `themes/yegsec/templates/schedule.tmpl`|
|Styles|`./themes/yegsec/assets/css/theme.css`|
|Top Bar/Nav|`./conf.py` and `./themes/yegsec/templates/base_header.tmpl`|

There's all kinds of other stuff you can do but those are the highlights and
you can read the Nikola docs for the real deal.

# Creating new posts

`nikola new_post -f commonmark`

That will create a new post markdown file that can simply be edited.

If you want you can override things like the post date at the command line. For more
info on new_post:

`nikola help new_post`


# Publishing the site
