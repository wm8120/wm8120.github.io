# wm8120.github.io
my personal website

## Use reveal.js html5 presentation framework
`reveal.js` is located in <website root>/reveal.js folder. It is added as a submodule of the website repository. Thus, it can be up to date through `cd reveal.js; git pull origin master`. In case we won't mess up the reveal.js/ repository, I recommand not to directly add or modify files in reveal.js/ folder. We can do as:
```
mkdir slides/
cd slides/
# ... new a slides.html ... #
```
It is necessary to use `<base>` tag for that all the relative paths in `slides.html` can be resolved as they start from the reveal.js folder. Here is the Usage:
```
<base href="http://<host>/path/to/base/" target="xxx"> or
<base href="/path/to/base/" target="xxx">
```
Add one of them into the `<head>` tag parcel. 

> The second usage may not be able to correctly parsed if the browser loads the local page through "file:///webfolder/slides/slides.html"
