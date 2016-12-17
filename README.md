# owo.sh

A basic example/uploader for uploading to owo.what-th.is's image server. The aim was to have a script that allowed for users of all operating systems (that werent already supported by ShareX) to also be able to upload to whats-th.is related products. 

Thank you to [jomo](https://github.com/jomo/) and his script [jomo/imgur-screenshot](https://github.com/jomo/imgur-screenshot), to which snippits and borrowing code guided me to improving my own script. This script wouldnt be anywhere near what it is today without his efforts.

# Install

## dependencies

| os         	 | dependency                   | description
|--------------- |----------------------------- |-----------------------------------------------------------------------------------------------------
| MacOS     	 | Terminal Notifier            | Default OSX Notifications suck and barely work, this is a workaround for that.
|      	     	 | Screencapture                | Comes default with OSX and is the client that you use when you press CMD + Shift 3 or CMD + Shift 4.
|      	      	 | Pbcopy                       | Comes default with OSX and is used to copy things to your clipboard.
|      	     	 | GREP                         | Comes standard with all UNIX os's and is used to (in this case) decipher JSON.
|      	     	 | cURL                         | Comes standard with all UNIX os's and is used to (in this case) upload to the owo server.
| Linux     	 | Notify-Send                  | Default Linux barely has any, if at all, notification support from terminal. This is a workaround.
|       	     | Maim                         | A rich screenshotting client, that better than what comes default with Linux.
|     	     	 | XClip                        | Comes default with most Unix based os's and allows for things to copied to clipboards.
|      	     	 | GREP                         | Comes standard with all UNIX os's and is used to (in this case) decipher JSON.
|     	      	 | cURL                         | Comes standard with all UNIX os's and is used to (in this case) upload to the owo server.

##instructions

1. Clone the repo with `git clone https://github.com/whats-this/owo.sh.git`
2. Make sure `script.sh` has permissions, `chmod a+x script.sh`.
3. Download the dependencies, you can check what you need with `./script.sh --check`
4. Put your token inside of `{HOME}/Documents/.owo/conf.cfg`, `nano {HOME}/Documents/.owo/conf.cfg`.
5. Run the command `./setup.sh` to add the owo command.
6. You can now run `owo file.png` from anywhere to upload `file.png`.

# Usage

Basic usage of the script is like so.

```shell
owo image.png
```

However the following flags can be placed after `owo` for the each of the results.

| short | command      	| description                              	|
| ----- |--------------	|------------------------------------------	|
| -h    | --help       	| Show the help screen to you,             	|
| -v    | --version    	| Show current application version.        	|
| -c    | --check      	| Checks if dependencies are installed.    	|
|       | --update     	| Checks if theres an update available.    	|
| -l    | --shorten    	| Begins the url shortening process.       	|
| -s    | --screenshot 	| Begins the screenshot uploading process. 	|

# Contribute

1. Fork repo.
2. Edit code.
3. Make a PR.
4. Submit said PR.

# License

A copy of the MIT license can be found in `LICENSE.md`.
