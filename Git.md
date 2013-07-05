# Git

Recreate a local copy of a remote tracking branch

    git checkout development
    git branch -D release
    git checkout --track origin/release
    
Checkout pull requests

    git config --add remote.origin.fetch '+refs/pull/*/head:refs/remotes/origin/pr/*'
    git checkout origin/pr/<pull request #>
