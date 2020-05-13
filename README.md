# SWIPL FLIPL -- Code / Test flipper.

This little extension will allow you to bind a key to a function
called `swipl-flipl` that simple, cleanly and very very naively finds
the file that is the dual of your current file in that if you are
editing the source file (*.pl) it will open the corresponding test
script (*.plt) file using the base filename as the stem.

## What it does

If you don't have a test script yet....it will open a file on a new
buffer for you as that's the standard Emacs behaviour when trying to
find a file that doesn't yet exist. Nothing to do with me but
nonetheless helpful :)

## Installation

Paste the code into your .emacs file and then bind a key like this:

    (add-hook 'prolog-mode-hook
          (lambda ()
            (local-set-key "\C-ct" 'swipl-flipl)))

That's Ctrl-C t, t for test or toggle or time-for-tea.

Of course, if you want to keep it separate etc then that's your
call. A mans .emacs file is his castle after all. (And that includes
ladies too of course, I didn't invent that expression).

## Issues, Requests etc.

Raise an issue...feel free to contribute.
