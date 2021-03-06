---
id: 63b184f7-1901-4580-af40-97ef87069a04
title: Local Preview
desc: ''
updated: 1600740884846
created: 1600740884846
stub: false
nav_order: 2.1
---
> The following guide was created by fellow Dendronite [Ed](https://github.com/ens100)! 

In order to publish your notes, we have included a brief step by step guide to get you started. 

In a nutshell, we need to:

- Install Ruby 
- Install Jekyll
- Set up the environment
- Publish our notes
- Enjoy the fruits of our labor

Although these may seem complex, I hope the following guide will assist and make things as simple as possible.

## Installing Ruby

Ruby version 2.5.0 or higher is needed, so open a Terminal window (eg. PowerShell / cmd) and type `ruby -v`. If the error message "_ruby : The term 'ruby' is not recognized_" comes up do the following:

- Navigate [here](https://rubyinstaller.org/downloads/) and download the recommended **Ruby+Devkit** and then open the downloaded file.
- When the installation is complete you will see an option to Run `ridk install`. Make sure this is checked as it is needed for installing Jekyll and click finish.
- A terminal window will open asking what components to install - Simply press the `enter` key to install the default components.
- Close the terminal and reopen a new iteration to ensure that the Path variables have been set.
- In the newly opened Terminal run `ruby -v` and you should get `ruby 2.6.6p146 (2020-03-31 revision 67876) [x64-mingw32]` or similar back.

## Installing Jekyll

- From the Terminal type `gem install jekyll bundler` and let it run until finished (takes a few minutes).
- When completed run `jekyll -v` and the Terminal should return with something like: `jekyll 4.1.1`.

Step 1 and 2 over and done with.

## Setting up the Environment

- In the Terminal navigate to the `docs` folder within your dendron vault.
  - The easiest way to do this is to copy the location of the folder in File Explorer and then go to the Terminal and type `cd ` and paste the copied text and then click enter. 
- Run `bundle install`

We are approaching the finishing line.

## Publishing Our Notes

In order for our notes / markdown files to be published we need to carry out the following steps:

- From within Dendron, run the "Build Pod" command by clicking `ctrl + Shift + P` and typing Pod. This will bring up the option `> Dendron: Build Pod`, select it and click enter.
- In the bottom right hand side after a few seconds you should see "finished".

## Last Step

- Open the terminal and type `bundle exec jekyll serve` 
- This will run a configuration to generate the markdown files to static pages so that they can be viewed online. 
- Once the above step is completed, open a web browser and navigate to `http://localhost:4000/`. 
- You should see a copy of your notes using a similar theme as this one.

You will be able to see any changes you do to your notes in Dendron on the localhost. 

Think this deserves a high five! 

