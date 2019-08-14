# tooter

a barebones mastodon client

## installation

- clone/download the repo
- `bundle install`
- modify `tooter.conf.example` to reflect your info*
- rename `tooter.conf.example` to `tooter.conf`
- `bundle exec ruby tooter`

*for instructions on how to get an access token for your account please [check here](https://github.com/theZacAttacks/silence#getting-an-access-token)

## usage

at the `Tooter>` prompt write anything and hit enter and it will be posted to your account

### keywords

to add content warnings or change the visibility of a post add a keyword into your post before you hit enter

supported keywords: `vis:`, `visibility:`, `cw:`, `spoiler:`, `reply:`

e.g., `Tooter> posting from tooter~ vis: unlisted cw: testing`, `Tooter> replying to a post vis: private reply: 11135863213` (assuming 11135863213 is a valid status id)

## commands

`!status <id>` -- returns a single status given an ID

`!notifs [amount]` -- returns AMOUNT of notifications (defaults to 10)

`!follow <account>` -- follows ACCOUNT after user confirmation

`!quit` -- quits the application

