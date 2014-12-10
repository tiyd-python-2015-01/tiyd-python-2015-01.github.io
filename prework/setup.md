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

* Install OSX Yosemite, if you haven’t already.
  1. You'll need to sign in to the Mac App Store with you Apple ID. If you don't have one, [sign up here](https://appleid.apple.com/).
  2. Download the Yosemite upgrade from the Apple Store: [download here](https://itunes.apple.com/us/app/os-x-yosemite/id915041082?mt=12).
  3. Double-click "Install OS X Yosemite” to begin installation.
  
  **WARNING:** The OS X upgrade can take a bit of time to complete and will require a restart. Plan on doing this in the evening or over a lunch break.

* Install Atom
  1. Download Atom from [the Atom website](https://atom.io/).
  2. Unzip the downloaded file by double-clicking on it. (It may be unzipped for you already, depending on how you downloaded it.)
  3. Move the Atom application into your Applications folder.
  4. Run Atom.
  5. Once Atom has started, click the Atom menu and run "Install Shell Commands."

* Install [Google Chrome](https://www.google.com/intl/en/chrome/browser/)

* Install XCode Command Line Tools
  1. Go to the [Apple Developer Downloads site](https://developer.apple.com/downloads/).
  2. You will have to register.
  3. Look for "Command Line Tools (OS X 10.10) for Xcode - Xcode 6.1.1" (Uploaded December 2014).
  4. Once downloaded, open the downloaded file by double-clicking on it. This should bring up a new window with a file that ends in .pkg. Double-click it and follow all the prompts.

* Install Homebrew
  1. Open up Terminal.app. If you have any trouble here, go through [the command-line prework](/prework/exercises.html#the-command-line).
  2. Run `ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"` and follow all the prompts.
  3. Run `brew doctor`
  4. Run `brew install readline`
  5. Run `brew install git`

* Create an SSH key (__do not__ give it a password when it asks for one)
  1. Run `ssh-keygen` in your terminal.

* Install pyenv
  1. Open up Terminal.app. If you have any trouble here, go through [the command-line prework](/prework/exercises.html#the-command-line).
  2. Run `curl -L https://raw.githubusercontent.com/yyuu/pyenv-installer/master/bin/pyenv-installer | bash`
  3. After this finishes installing, type `atom ~/.bash_profile`.
  4. Copy and paste the following lines into `.bash_profile`:

          export PATH="$HOME/.pyenv/bin:$PATH"
          eval "$(pyenv init -)"
          eval "$(pyenv virtualenv-init -)"

  5. Save the file and close Atom.
  6. Close your Terminal window.
  7. Open a new Terminal window.
  8. Run `pyenv doctor`. You should see "Congratulations! You are ready to build pythons!"
  9. Run `pyenv install 3.4.2`. This will take a while.