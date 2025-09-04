---
layout: project
type: project
image: img/director/thumb.png
title: Director
date: 2023
published: true
labels:
  - Neovim
  - Code Editor
  - Plugin
summary: "A Neovim plugin for creating smooth, configurable workflows."
---

Neovim is a terminal-based and highly configurable code editor that lacks the features of a standard IDE. My project Director is my attempt at enabling Neovim to function as a stand-alone development environment. Director comes with little functionality of its own, but provides a framework for creating workflows and actions using lua. Workflows are configurable at runtime and can be saved to disk (when enabled) to use later. For instance, I created a Director workflow CMake, that allows users to specify which flags to pass to the build command. I also created a workflow for TypeScript that automatically runs `tsc --watch` whenever a TypeScript project is detected.

I am the sole developer of Director, and have written extensive documentation detailing how to use the tool. The project was an adventure in terminal UI and UX design that required me to think critically about making the plugin efficient as possible to use, and easy to configure. I also learned how to write engaging and informative API documentation in the process.

The source code can be found [here](https://github.com/SamManibog/director) along with documentation and installation instructions for Lazy, one of Neovim's package managers.
