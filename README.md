# Mac Setup
Quickly setup most of the tools that you need for development.  If you don't trust the script, you're welcome to just look and see what tools are installed so that you can manually choose them instead.  This was done on an Apple Silicon Mac.  It might work fine on an older one but YMMV. /shrug

Get started:
  1. Log in on your device with your icloud account first
  2. Open a terminal
  3. Run `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"` to install brew
  4. Install git: `brew install git`
  5. Clone this repo and cd into the root
  6. Install ansible: `brew install ansible`
  7. Run `ansible-playbook main.yaml`

## Notes on asdf
If you're not familiar with [asdf](https://asdf-vm.com/guide/introduction.html) I recommend reading up on it a bit.  It's basically a really useful version manager that works with many different languages / tools.  Depending on what repo/directory you're working in in the future, you may need to run `asdf install` to ensure that you have the correct versions for the required pacakages of that repo that are mentioned in the `.tool-versions` file in the directory that you are in.

## Notes on vscode plugins
It is assumed that vscode plugins are a fairly personal choice.  None are installed by this script.  Because of this, it's recommended to just sync your plugins with your account and then you can use them on any machine you use in the future.

## Notes on customization
There's probably still going to be some customization that you'd like to do on your machine (for the dock, look at feel, other random settings for example).  This is also fairly personal and isn't high value to automate.  Feel free to touch things up as you deem appropriate.

That's pretty much it.  This should install pretty much everything you need.