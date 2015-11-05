# Hiro Start File

The concept behind start files was born from several things:

* wanting to find/open files without being hindered by tab-completion and slow
  fuzzyfinder plugins
* wanting to have frequently performed tasks readily available
* knowing how efficient vanilla vim can be
* vim not always doing what vim does best

## What does a Start File Contain

A start file contains a few things:

1. The list of non-gitignored files in the project (or all files, if you want)
  * this way you can find any file with a simple regex, and open it with 2
    keystrokes (`gf` or `<c-w>f`)
  * or possibly sorted by either how frequently they are modified, or how
    recently they were modified
  * using vim's command-mode your ability to quickly access a file is often
    slowed by tab-completion stopping you at every directory level
  * slow indexing times of fuzzyfinders can also be frustrating
2. The current `git status` prepared with `git add` so you can quickly make the
   list of what you want to add, and run it, all with only a few keystrokes.
3. A customizable list of commands frequently ran with this project.
  * vim's closeness with the shell makes it effortless to use unix as an ide.
    it offers at least 3-4 ways of not only running shell commands, but also
    interacting with and manipulating the data returned.

## Other features

* The ability to refresh/update a start file should only be a keymapping away

## Future Possibilities

* The ability to customize the template/format of a start file
  * prepackaged configurations by app-type (rails, django, etc.) could improve
    adoption rates

