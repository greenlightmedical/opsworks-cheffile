# Setup

This will allow you to use [librarian-chef](https://github.com/applicationsonline/librarian-chef) to manage your OpsWorks cookbook dependencies as you would rubygems in a Gemfile. Edit the `Cheffile` to your heart's content with the custom cookbooks that you need to use. The `Cheffile` in the repository contains the custom cookbooks that we currently use at [Cult Cosmetics](https://www.cultcosmetics.com).

1. Clone this repo
1. `bundle`
1. `thor list`

## How to use

1. `thor cookbooks`
1. `thor cookbooks:install`
1. `thor cookbooks:package`
1. `thor upload ACCESS_KEY SECRET_KEY BUCKET [REGION]`

### Notes
- `thor cookbooks:update` does not seem to function properly -- if needing to reset or update pkgs, just remove ./cookbooks and ./tmp directories and start over
