#Arduino Tutorial Resources

A set of resources for teaching basics of Arduino programming and circuitry. This is an attempt to centralise these reusable resources and also iterate and improve them with feedback from workshop participants and facilitators. Attempting to be consistent in style and conventions when it comes to coding, breadboard use and circuitry.

## Code
All source code provided under GPL v3. Each tutorial in it's own directory containing the ino file and any other source files.

## Fritzing
Fritzing diagrams and source files also provided.

## Github Pages

Also taking advantage of the free hosting on [Github Pages](http://pages.github.com/). There is a `gh-pages` branch for this project that has a [Jekyll](http://jekyllrb.com/) base site. This page renders here: [http://opensystemsassociation.github.io/arduino-tutorial-resources](http://opensystemsassociation.github.io/arduino-tutorial-resources). The [Blink page](http://opensystemsassociation.github.io/arduino-tutorial-resources/blink) for example uses the Fritzing diagram that lives in the `master` branch `blink` directory and the code being displayed is also the latest version from the Github repository `master` branch.

To create a new page for a new tutorial you need to create a directory for your tutorial on the `master` branch then add the code and Fritzing images. After this you will need to `merge` the `master` branch into the `gh-pages` branch:

```bash
$ git checkout gh-pages
$ git merge master
```

Once you've done this you will need to create a new file in the `_posts/` directory. The file name must start with the date (parts delimited by hyphen) and be followed by the name of the tutorial (which will determine the url of the page).

See the [blink example file](https://github.com/opensystemsassociation/arduino-tutorial-resources/blob/gh-pages/_posts/2013-12-19-blink.markdown) in `_posts/` as an example.
