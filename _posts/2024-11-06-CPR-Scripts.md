---
title: Scripts I use to run Cyberpunk Red
categories: [Cyberpunk Red, Tools]
tags: bash, python, github, gm-ing
media_subpath: /assets/img/cpr-scripts/
---

Running Cyberpunk Red can be a pain in the ass. Don't get me wrong they did a lot of work slimming down the existing Cyberpunk rules, but there are so many little things to roll especially with all the DLC. There are lots of tools to help like the Cyberpunk Red Companion app[^companion] but a nicely designed little app isn't exactly *cyberpunk* (also that app is a little slow to update). What is cyberpunk are shell scripts!

This post is going to serve as a rolling list of what scripts I am using to run my online games, so I will come back and add stuff as I find it. Now without further ado, *the scripts*.

# Bash

So far the only bash script I use for running games is a dice rolling function from the excellent (if still unreleased) zine **Script Wizards**[^script-wiz]. Now technically this is a Python script that pipes the output into **glow**[^glow] to make it pretty. So in addition to **glow** you need the Python package **d20**[^d20-py].

```bash
function dice () {
        if [ -n "$1" ]; then
                local cmd
                cmd="from d20 import roll;
print(str(roll('$1')))"
                python -c "$cmd" | glow -
        else
                echo "Missing statement"
        fi
}
```

It's pretty simple but the output is pretty and readable.

![Dice script output]({{ page.media_subpath }}dice_script.webp)

# Python

These are straight Python scripts. Alias those bad boys and you have some instant power in your shell. For those wanting to replicate my setup, I clone the git repos for these scripts into a `~/.scripts` folder and then add aliases to my `.bashrc`. I will include the alias for each script as well.

## Net-arch generator [^net-gen]

![netarch output]({{ page.media_subpath }}netarch.webp)

Your netrunner is out to get you. We all know it. That bastard will find net-archs you never planned for and expect to sit there and hack the damn thing. This script lets you blast out a whole arch in moments to deal with their plug-head addiction.

```bash
alias netarch='python ~/.scripts/Cyberpunk-Red-Net-Arch-generator/net_arch_gen_2.0.py'
```

## Gunpath [^gunpath]

![gunpath output]({{ page.media_subpath }}gunpath.webp)

This one is of my design. The Toggle's Temple[^togs] DLC introduced the gunpath for adding gun flavour. It's cool but a lot of work, and this removes that hassle and adds in its place flags to theoretically save time.

```bash
alias gunpath='python ~/.scripts/CyberpunkRedGunGenerator/CyberpunkRedGunGenerator.py'
```

[^companion]: https://cyberpunkred.com/#/
[^script-wiz]: https://scriptwizards.itch.io/issue-1
[^d20-py]: https://pypi.org/project/d20/
[^glow]: https://github.com/charmbracelet/glow
[^net-gen]: https://github.com/benjo121ben/Cyberpunk-Red-Net-Arch-generator
[^gunpath]: https://github.com/LukeOssevoort/CyberpunkRedGunGenerator
[^togs]: https://rtalsoriangames.com/wp-content/uploads/2024/06/RTG-CPR-DLC-TogglesTemplev1.1.pdf
