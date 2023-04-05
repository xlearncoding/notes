---
title: Install git
---

To begin using Git, you must first install it on your computer. The installation process will differ depending on your operating system. I will guide you through the steps for each operating system, including Windows. It's worth noting that you don't need to change your operating system at this point in your coding learning journey. However, unless you decide to continue with the .Net Framework, I do recommend using Unix-like operating systems such as MacOS or Ubuntu as you progress further in your learning journey.

Before you start working with Git, it's important to check if it's already installed on your computer. If you're using MacOS or any Linux distribution like Ubuntu, you can check by [[open your terminal|opening the terminal]] (if you're using Windows, you can check by [[open your Command Prompt|opening the Command Prompt]]) and typing,

```bash
git --version
```

If Git is installed, you will see the version number displayed, for example:

```bash
> git version 2.30.1 (Apple Git-130)
```

However, if you see an output like 

```bash
> command not found: git
```

you'll need to download and install git.

For ==MacOS users==, you can install Git using Homebrew, a package manager for macOS. To install Homebrew, open the Terminal and run the following command:

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

Once Homebrew is installed, you can install Git by running the following command:

```bash
brew install git
```

For ==Ubuntu users==, you can install Git using the apt package manager. Open the terminal and run the following command:

```bash
sudo apt-get update
sudo apt-get install git
```

For ==Windows users==, you can download the Git installer from [the official website](https://git-scm.com/download/win). Once the installer is downloaded, double-click it to start the installation process. Follow the prompts to complete the installation.

Once you've installed Git, you can check that it's working correctly by running the `git --version` command again in your terminal or command prompt. If the version number is displayed, you're ready to start using Git!

Next: [[courses/git/git practise|Basic git practise]]

---

[[courses/git/Mini Course git|Mini Course: git]]
* Introduction
	- [[courses/git/What is git?|What is git?]]
	*  [[courses/git/Why is git important?|Why is git important?]]
	 * [[courses/git/Basic git terminology|Basic git terminology]]
 * Install git and practise
	 * [[courses/git/Install git|Install git]]
	 * [[courses/git/git practise|Basic git practise]]
