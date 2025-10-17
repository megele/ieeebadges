# ieeebadges.sty --- affix IEEE Security & Privacy Artifact Evaluation badges

The `ieeebadges` LaTeX style file affixes IEEE Security & Privacy Artifact
Evaluation badges to the front page of your IEEE-formatted paper.

## INSTALLATION

Put `ieeebadges.sty` and the `ieeebadges-*.pdf` graphics files in
the directory that contains the LaTeX source for your paper.  (Really,
you can put them anywhere in LaTeX's search path, but the simplest
thing is to put the files in the same directory as your paper's LaTeX
source files.)

## USAGE

In the preamble of your LaTeX document, insert a line like this:

```
  \usepackage[<options>]{ieeebadges}
```

In the options, list the badges that have been awarded to your paper.
The possible badges are:

  * `available`  --- affix the "Artifacts Available" badge
  * `functional` --- affix the "Artifacts Functional" badge
  * `reproduced` --- affix the "Results Reproduced" badge

Example:

```
  %% Affix the indicated badges to the paper.
  \usepackage[available,functional]{ieeebadges}
```

Tips:

In your LaTeX document, the `\usepackage[...]{ieeebadges}` directive
must come after `\documentclass` and before `\begin{document}`.

If your LaTeX document has many `\usepackage` directives, put
`\usepackage[...]{ieeebadges}` near the end of those.  This may
avoid problems relating to conflicting options for the `graphicx`
package.
