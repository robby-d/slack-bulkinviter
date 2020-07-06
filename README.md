# slack-bulkinviter

Super quick and dirty Python script to bulk invite ALL users in a slack team to a specific channel. We need to do this regulary with [Counterparty](http://www.counterparty.io) when we create a new channel that everyone should be in, or move things around.

To use:
* Install the [slacker](https://github.com/os/slacker) library via `pip`
* [Get an API key](https://get.slack.help/hc/en-us/articles/215770388-Creating-and-regenerating-API-tokens)
* Optionally, if not using `--apikey`, create a file in the same directory as `slack-bulkinviter.py` containing your API key and pass the filename to the argument `--apikey` or `-k`
* Execute the script, passing the name of the channel where all users will be invited, such as `./slack-bulkinviter.py --channel mychannel --apikey myapistring`
* Sit back and let it do its work

Also, here's a best practice that any Slack workspace member can do very quickly directly in Slack. No Python script required.

1. Type the `/who` command in a channel where you most of the people you want to add already hang out
2. Copy the output
3. Paste it in the channel where you want to invite them
4. Press Enter

Slackbot tells you that you have mentioned people who "are not in this channel" and gives you an `Invite Them` button.

_Hat tip: [jonareyes at StackExchange](https://webapps.stackexchange.com/a/123420/36481)_
