Making git nicer to work with on OS X

# Installation
This repo just packages up a few git tools (thanks to Shawn O. Pearce) and a common profile for use with Mac OS X. The easiest way to use this repo, from your home directory:

1. ln -s [path-to-repo]/git-completion.sh .git-completion.sh
2. ln -s [path-to-repo]/git-prompt.sh .git-prompt.sh
3. Add the top of profile.example to your ~/.profile.
4. (Optional) Add the rest of profile.example to your profile.

Instead of symlinking, you could instead copy git-completion.sh and git-prompt.sh to ~/.git-completion.sh and ~/.git-prompt.sh respectively.

If using the PS1 in profile.example, when you start a new terminal session your prompt should be:
yourname@yourcomputer:full/current/path $ [ with nice, pretty colors ]

If you're in a git repo, you should see:
yourname@yourcomputer:full/current/path (current_git_branch)$ [ with nice, pretty colors ]

If you don't want to use the given PS1, or you want to show repo status as well as branch, see git-prompt.sh for more details