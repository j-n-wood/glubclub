+++
date = '2026-03-24T12:22:14+13:00'
draft = false
title = 'Celestia build'
+++

# Building Celestia

## Why

So I thought that for some project I wanted to play with, I could use images of the planets in the solar system.

Searching around for free sprite sheets or similar didn't find what I wanted.

Asking tools to generate something also didn't produce what I wanted.

Then I remembered Celestia, the virtual observatory program. It can take screenshots of any body in the solar system. Perhaps that would do what I wanted, and I can use image tools or scripts to build a sprite sheet of icon size images if I need to.

## Attempt 1

On a Mac laptop, I installed Celestia from the app store. Works out of the box. Scripting to zoom to a planet and take a screenshot works - except the screenshot won't save.

Chatting with the bots came up with a bunch of options to attempt to grant permissions and allow the app to write to a target folder - all fail. Well, I didn't really want to work on the laptop anyway, so I figure when I get back home I'll use my linux machine and can set up what I need there.

Since then I've found out enough that I may be able to fix the issue now - but as I don't want to work in that environment anyway, I haven't checked.

## Attempt 2

On linux, clone the repo. Configure and build. Deal with the bunch of dependencies (install instructions for linux are old but roughly enough).

Get the current branch building. Hooray. Bot suggests a lua script to visit the various target bodies and take screenshots.

Script immediately fails. Seems that the lua script docs are well out of date. Bot suggests listing members of the tables to work out methods that _are_ available. Or downgrade to a 'stable' version that matches the docs.

## Attempt 3

See if there is a 'stable' version that matches the docs. Prior release tag checked out - build system is different. Deal with that, and find that windowing system is also different. Can make a UI-less GLUT build. That works, screenshots might save - but going where? And the key commands to run a script - don't work?

## Attempt 4

Why bother with old window systems - back to the current build. Stop relying on the bot to figure things out. I have the code.

* bung a log line in the screenshot saving path, backtrack to the config file entry that controls the output path.
* find the lua script binding methods. Now I can see what the current version of the script entries are, and what their parameters do.
* point a bot to scrape the lua bindings and make cheatsheet docs of methods and their parameters, and list the enums for things like the renderFlags that control what is visible.

Test scripts now work. I can reliably change them and make new calls that are correct.

Make a script to visit various bodies in turn and save screenshots without clutter.

Make a shell script to use imageMagick to make a montage image of smaller size versions.

Success!

Lesson - don't lean on the chatbots. Read the install/readme.md. Use the source.
