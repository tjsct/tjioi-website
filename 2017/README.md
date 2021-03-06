# TJ IOI Website
The website for TJ IOI 2017. Currently, TJ IOI is being run by SCT. If you'd like to help out, contact the SCT officers.

Note that this repo is automatically deployed to https://tjsct.github.io/tjioi/. However, the official website is https://activites.tjhsst.edu/tjioi/, which requires someone to manually pull the Git repo. Don't be too afraid to push commits to the repo: they won't automatically go up on the official URL!

Some general guidelines:

* Keep it professional, please. This is going to be seen by potential sponsors and teachers from other high schools. Your words reflect on TJ.
* Prefer to use existing Bootstrap styles over writing your own CSS.
* To create links: `<a href="{{ '/registration/' | relative_url }}">Registration</a>`. Because Jekyll. And because the base URL changes.
* Currently, indentation is kind of inconsistent. Use either two or four spaces, and be consistent with the surrounding code. If you use three spaces, this incident will be reported.

## Setting up Jekyll
This site runs on Jekyll. To use that, first you need to install Ruby and DevKit or whatever. If you're on Ubuntu/Debian, run `apt-get install ruby ruby-dev`. If you're on Windows, try following the instructions at https://labs.sverrirs.com/jekyll//1-ruby-and-devkit.html, and good luck.

Next, you need to install Jekyll. Open a command prompt, and run `gem install bundler jekyll`. Then `cd` to the cloned repo, and run `bundler install`. If you don't have sudo, you'll need to find the location of the Jekyll binary, probably in `~/.gem/ruby/2.0.0/bin` (change version number).

You should now be able to run `jekyll serve --incremental` to run the project as a web server.
