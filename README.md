# slack-bulkinviter

Super quick and dirty Python script to bulk invite ALL users in a slack team to a specific channel. We need to do this regulary with [Counterparty](http://www.counterparty.io) when we create a new channel that everyone should be in, or move things around.

To use:
* Install the [slacker](https://github.com/os/slacker) library via `pip`
* [Get an API key](https://get.slack.help/hc/en-us/articles/215770388-Creating-and-regenerating-API-tokens)
* Create a file in the same directory as `slack-bulkinviter.py` called `apikey.txt`, containing your API key
* Execute the script, passing the name of the channel where all users will be invited, such as `./slack-bulkinviter.py mychannel`
* Sit back and let it do its work
