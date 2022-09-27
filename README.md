# test-automatic-changelog
A test repo for how to better generate an automatic changelog

I will also describe how to set up an automatic changelog generation with https://github.com/github-changelog-generator/github-changelog-generator.

You have to set it up locally, as it is a ruby gems that we need to install : ```gem install github_changelog_generator```, if you do not have ruby have a look here : https://www.ruby-lang.org/en/ to install it, if it is already installed you may want to upgrade it to a version higher to 3.0 and install additional dependencies.

For a simple test, go to your repo and type : ```github_changelog_generator -u sasip-climate -p test-automatic-changelog```, it will generate a CHANGELOG.md file like [this one](https://github.com/sasip-climate/test-automatic-changelog/blob/main/CHANGELOG.md)

For more informations on the releases and following : https://github.com/Ic3fr0g/autochangelog-hook, you can set up a git hook :
  - download the scripts in https://github.com/Ic3fr0g/autochangelog-hook/tree/master/git/hooks
  - put them in the .git/hooks of your repo
  - modify https://github.com/Ic3fr0g/autochangelog-hook/blob/master/git/hooks/run_changelog.sh so it fits your need
  - a [new CHANGELOG](https://github.com/sasip-climate/test-automatic-changelog/blob/main/CHANGELOG_append.md) is generated with more informations for the releases
  - it will then automatically generate the changelog when a merge is done on the main branch ?


