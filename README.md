# A theme for Taskpaper for those who use notes more than tasks

[Taskpaper 3](http://www.taskpaper.com) is about to come out, and here's a theme for those who:

* Use *note* items a lot, and tasks (dashed items) just a little
* Find the handle (the circle next to the lines) handy mostly to collapse indented items
* Prefer URLs to appear discreetly, but still look clickable
* Prefer to use the keyboard to cut-paste items to re-order them over using draggable handles to re-order items (on the Mac anyway)

## Installation

In your terminal:

    # Download theme to Application Support directory
    cd ~/Library/Application\ Support/Taskpaper/
    git clone https://github.com/pascallaliberte/theme-notes-first.git

    # Backup the previous theme.less and copy theme.less from theme-notes-first
    mv theme.less theme-backup.less && cp -p theme-notes-first/theme.less theme.less

You can still make adjustments to the theme, and upgrade it when there are new updates (see [Upgrading](#Upgrading) below).

## Here's how it looks

![Preview of a taskpaper with the theme applied](preview.png)

## Upgrading

Since `theme.less` gets copied from the `theme-notes-first` directory, you can still make your own adjustments.

When upgrading, a copy of your `theme.less` gets saved to `theme-backup.less`

    # Download the latest version of the theme
    cd ~/Library/Application\ Support/Taskpaper/theme-notes-first
    git pull origin master

    # Backup the previous theme.less and copy theme.less from theme-notes-first
    cd ~/Library/Application\ Support/Taskpaper/
    mv theme.less theme-backup.less && cp -p theme-notes-first/theme.less theme.less

To get notified of updates, [subscribe be notified by email](http://pascallaliberte.me/uses-taskpaper/).

## Collaborating

1. Use a symlink to point to the theme.less inside the theme-notes-first directory

  ```
  cd ~/Library/Application\ Support/Taskpaper/
  mv theme.less theme-backup.less && ln -s theme-notes-first/theme.less
  ```

2. Fork this project
3. Create a branch with your new change e.g. `use-variables-everywhere`
4. Push your branch
5. Submit a pull request for your new branch

## Thanks

Thanks [Jesse Grosjean](http://www.hogbaysoftware.com/about) for working on version 3. I'm so glad Taskpaper exists!
