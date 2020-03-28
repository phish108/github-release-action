# github-release-action

Create github releases from your commits.

This action creates github releases from your actions.

`github release` is designed with simplicty in mind. It will use your github comments, tags, issues, and prior releases to create the release info for you. 

This action automatically launches, if the latest tag in you repository is a `semver`-tag. It is designed to integrate with my [`Autotag`-action](/phish108/autotag-action) for release action. 

`GitHub release` will fetch the last release for your repository and creates a release title and release infos from your commits.

The action checks for #major, #minor, #patch, and `fixed`-commits and build a structured release information for you. If you follow the "clean code"-"agile programming" paradigm of working from issues and close them via GitHub's `fixed` commit message syntax, this action will use your issue labels and and issue titles to create your release information for you. 

The action creates release titles for you to indicate breaking API or UI changes, enhancements, or new features. For patches, bug fixes, dependency bumps, and unlabeled commits, it uses a simple enhancements.


