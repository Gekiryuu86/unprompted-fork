# Unprompted for Stable Diffusion
Supercharge your prompt workflow with this powerful scripting language!

![unprompted_header](https://user-images.githubusercontent.com/95403634/199041569-7c6c5748-e7dc-4068-943f-c2d92745dbb5.png)

## Introduction

**Unprompted** is a highly modular addon for [AUTOMATIC1111's Stable Diffusion Web UI](https://github.com/AUTOMATIC1111/stable-diffusion-webui) that allows you to include various shortcodes in your prompts. You can pull text from files, set up your own variables, process text through conditional functions, and so much more - it's like wildcards on steroids.

While the intended usecase is Stable Diffusion, **this engine is also flexible enough to serve as an all-purpose text generator.**

Still under active development - I am excited to read your feedback but please keep in mind that this is an early release!

> Unprompted is built on top of Darren Mulholland's excellent [Python Shortcodes](https://www.dmulholl.com/dev/shortcodes.html) library.

## Installation

Simply clone or download this repo and place the files in the base directory of Automatic's web UI.

> **💡 Tip:** You can run the included `unprompted_dry.py` to generate text in Command Prompt without needing Stable Diffusion. No external dependencies required!

## Basic Usage

From either the txt2img or img2img screen, select Unprompted as your active script:

![unprompted](https://user-images.githubusercontent.com/95403634/198924886-da1bd887-5e9f-4c29-a321-0bb1b590a327.png)

Now, shortcodes in your prompt will be processed through Unprompted to assemble the final string for image generation.

### Trying out the included demo

Enter the following as your prompt:

`[file human/main]`

> **💡 Tip:** This is a simple "human generator" that will choose characteristics like hair color, race, and posture.

The `[file]` shortcode looks in `unprompted/templates` for the specified text file (in this case `unprompted/templates/human/main.txt`.) You do not need to type the file extension.

Example output:

![image](https://user-images.githubusercontent.com/95403634/198927183-d98cdbb9-dab5-4623-9e1f-b77a0292714e.png)

## Learn More

There are too many features to include on one page!

To learn more about what Unprompted is (and isn't) capable of, please check out the following resources:

- [Starter Guide](../docs/unprompted/GUIDE.md)
- [Full Documentation](../docs/unprompted/DOCUMENTATION.md)
- [Changelog](../docs/unprompted/CHANGELOG.md)

For an example of a working, sophisticated template, you can [check out the inexpensive Fantasy Card Template here](https://payhip.com/b/hdgNR). Purchases will help continue to fund this project. ❤

> 🔧 If you run into a problem, feel free to [open an Issue.](https://github.com/ThereforeGames/unprompted/issues)

> 💬 For general discussion and template sharing, use [our Discussions board.](https://github.com/ThereforeGames/unprompted/discussions)