# Lesson 1 - Getting your development environment setup

## Installing your code editor

The first thing we need to do is get you setup to start running code. To do this we need a code editor. You *can* use any text editor to code since we are writing text into a file which will be run by another application, but people have done a lot of good work to create special text editors to work with code so that they do things like call out your mistakes and let you run code more easily.

For these lessons we will be using [VSCode](https://code.visualstudio.com/) since it's available for all major platforms and free. Go to the [download](https://code.visualstudio.com/Download) page and pick the version for your operating system.

### The terminal

In VSCode the terminal can be called up by using `ctrl + ~` on a standard keyboard and `cmd + ~` on Mac #thinkdifferent.

On Windows you should install [git bash](https://gitforwindows.org/) as your terminal because it contains most of the commands you will find on a Linux or Mac environment along with installing [Git](https://git-scm.com/) which is used to version your code so you don't have to do `ctrl/cmd + z` constantly.

## Installing Node with NVM (Node Version Manager)

[Node](https://nodejs.org/en/) is a program that runs JavaScript code. Once we have the files ready in our editor we will use the console to execute. NVM is the easiest way to install Node 

### Mac & Linux

1. Follow the [install instructions](https://github.com/nvm-sh/nvm#install--update-script) by running the command in your terminal.
2. Run `nvm install --lts`
3. Run `npm install -g avn avn-nvm avn-n`
4. Run `avn setup`

### Windows

1. On Windows we are actually going to use [Volta](https://docs.volta.sh/guide/getting-started) as that is the preferred option for this tutorial.
2. Run `volta install node`

## Verify install

You should now be able to run `node -v` in your terminal which should output the current node version installed.

```bash
$ node -v
v14.17.4
```
