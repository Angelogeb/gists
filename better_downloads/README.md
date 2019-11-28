### What is this?

A script that moves downloaded files in specified subfolders based on their
extension.

### Eeew, why not use filetype signatures as `file` does?

By extension works _most of the times_ and doesn't require opening the file.

### Why should I need it?

If you compulsively download from _legal_ sources only such as arXiv your
`Downloads` folder can get quite cluttered.

### How does it work?

It uses `pyinotify`. It works on my Linux machine™ with some version of
Chrome and Firefox as long as `IN_ATTRIB` is close to the last event performed.


### Couldn't this be done in plain `bash/zsh/ksh/kash/fish/llamas/<favourite_shell>`?

That's what this aims for, someone to point out a script that does this without
needing Python `>=3.4`.


### What's the worst that can happen using it?

Nothing, at least _so far_.

### How do I change download folder or extensions/subfolders?

Change `downloads` and `destinations` in the script.

#### Bold move not providing a proper way to configure that in a world where [dhall](https://dhall-lang.org/) exists

Agree

### How to run

`./better_downloads`

### How to kill
`kill $(cat /tmp/better_downloads.pid)`
