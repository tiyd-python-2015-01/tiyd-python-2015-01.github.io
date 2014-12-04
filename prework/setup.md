---
layout: default
---

## Mac Setup

As soon as possible after receiving your Mac, run through the following steps.
If you've done a lot of your own configuration, some of these steps may have to
change.  If you run into ANY PROBLEMS, send me an e-mail at:

clinton@theironyard.com

Again, we want to have all of these kinks worked out in advance, so PLEASE
e-mail if things don't work as described below.

* Install Atom
  * Download Atom from [the Atom website](https://atom.io/).
  * Unzip the downloaded file by double-clicking on it. (It may be unzipped for you already, depending on how you downloaded it.)
  * Move the Atom application into your Applications folder.
  * Run Atom.
  * Once Atom has started, click the Atom menu and run "Install Shell Commands."

* Install Google Chrome
  * Get it [here](https://www.google.com/intl/en/chrome/browser/).

* Install XCode Command Line Tools
  * Go to the [Apple Developer Downloads site](https://developer.apple.com/downloads/).
  * You will have to register.
  * If you are running Mavericks, look for "Command Line Tools (OS X 10.9) for Xcode - Xcode 6.1.1" (Uploaded December 2014).
  * If you are running Yosemite, look for "Command Line Tools (OS X 10.10) for Xcode - Xcode 6.1.1" (Uploaded December 2014).
  * Once downloaded, open the downloaded file by double-clicking on it. This should bring up a new window with a file that ends in .pkg. Double-click it and follow all the prompts.

* Install Homebrew
  * Open up Terminal.app. If you have any trouble here, go through [the command-line prework](/prework/exercises.html#command-line).
  * Run `ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"` and follow all the prompts.
  * Run `brew doctor`
  * Run `brew install readline`
  * Run `brew install git`

* Create an SSH key (__do not__ give it a password when it asks for one)
  * Run `ssh-keygen` in your terminal.

* Install pyenv
  * Open up Terminal.app. If you have any trouble here, go through [the command-line prework](/prework/exercises.html#command-line).
  * Run `curl -L https://raw.githubusercontent.com/yyuu/pyenv-installer/master/bin/pyenv-installer | bash`
  * After this finishes installing, type `atom ~/.bash_profile`.
  * Copy and paste the following lines into `.bash_profile`:

        export PATH="$HOME/.pyenv/bin:$PATH"
        eval "$(pyenv init -)"
        eval "$(pyenv virtualenv-init -)"

  * Save the file and close Atom.
  * Close your Terminal window.
  * Open a new Terminal window.
  * Run `pyenv doctor`. You should see "Congratulations! You are ready to build pythons!"
  * Run `pyenv install 3.4.2`. This will take a while.
