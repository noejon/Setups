# Setup for MacOs

## Browsers

Daily use: [Arc](https://arc.net/)

Development:

- Chrome (although arc is Chromium based)
- Firefox
- Safari

## Terminal

Started to use [Warp](https://www.warp.dev/)
Used to use Hyper before.

## ZSH

### oh-my-zsh

Install [oh-my-zsh](https://ohmyz.sh/#install):

```sh
sh -c "$(curl -fsSL <https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh>)"
```

## GIT

Normally comes pre-installed on latest MacOS builds. In case it does not just follow the [installation instructions](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git).

### Connecting to github

I usually always go back to [this page](https://www.atlassian.com/git/tutorials/git-ssh) from Atlassian. I just use a ed25519 key instead as it is shorter and safer and everyone should be using this.

```zsh
ssh-keygen -t ed25519 -f ~/.ssh/private-noj -C "Comment for the Key, good to identify it"
eval "$(ssh-agent -s)"
ssh-add -K ~/.ssh/name-of-the-key
cat ~/.ssh/name-of-the-key.pub
```

> Note: surely there is a command that you once knew and forgot that copies the content of cat for you to paste directly

Copy the content of cat and paste it as the new key in GH

## IDE

[VS Code](https://code.visualstudio.com/)

I like [launching code from the command line](https://code.visualstudio.com/docs/setup/mac#_launching-from-the-command-line)

- Launch VS Code
- Open the command palette (`Cmd+Shift+P`) and type `shell command` to find the `Shell Command: Install 'code' in PATH`
- Restart the terminal for the `PATH` to take effect

### Extensions

TODO: Add lists of extensions I am using
TODO2: Time for a review!

## node

Some peops brew it, I usually use [nvm](https://github.com/nvm-sh/nvm).

Xcode command line tool needs to be installed as a pre-requisite.

## pnpm

Remember the days when you used IE to install firefox or chrome:

```zsh
npm i -g pnpm
```

## Font - Victor Mono

I quite like Victor Mono, a nice open source font, that I use for coding.

Once downloaded and unzipped, open `font book` (installed by default on mac) and drag and drop the unzipped Victor Mono folder to it.

## What did I miss?
