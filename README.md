# dotfiles
:hocho: .files

My baby steps in dot files and Unix systems, using a Mac.

## Installation

**Warning:** If you want to give these dotfiles a try, you should first fork this repository, review the code, and remove things you don’t want or need. Don’t blindly use my settings unless you know what that entails. Use at your own risk!

### Using Git and the bootstrap script

You can clone the repository wherever you want. The bootstrapper script will pull in the latest version and copy the files to your home folder.

```bash
git clone https://github.com/thodorisbais/dotfiles.git && cd dotfiles && source bootstrap.sh
```

To update, `cd` into your local `dotfiles` repository and then:

```bash
source bootstrap.sh
```

Alternatively, to update while avoiding the confirmation prompt:

```bash
set -- -f; source bootstrap.sh
```

## Local changes
- For any new update on the `.bash_profile`, ensure that you run `bash -l` afterwards, so that the changes take effect.
- Scripts under /usr/local/bin have to have the proper permissions, so that they can be run outside of the latter directory (=globally). Ensure that by `chmod 755 [name-of-the-newly-added-script]`

## Thanks to…

* [Mathias Bynens](https://github.com/mathiasbynens) and his [dotfiles repository](https://github.com/mathiasbynens/dotfiles)
