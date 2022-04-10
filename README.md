# PAW Reddit Tipbot
 is a reddit tipping service to easily give PAW to your favorite redditors! [PAW](https://paw.digital is a feeless, instant, fun cryptocurrency. Before using PAW Tipper, please take a look at the [Terms of Service](https://github.com/SecureChainFinance/paw_reddit_tipbot#terms-of-service)

It is a fork and modification of the [Nano](https://nano.org) reddit tipbot created by /u/zily88 - which is available on [GitHub](https://github.com/danhitchcock/nano_tipper_z)

### To get started with PAW Tipper, either:
A) **Create an account** by [sending a message](https://reddit.com/message/compose/?to=paw_tipbot&subject=command&message=create) to /u/banano_tipbot with 'create' or 'register' in the message body. You will receive a PAW address, to which you can add PAW\*.
\-or-
B) **Receive a PAW tip** from a fellow redditor, and you will automatically have an account made! be sure to activate it afterwards by [sending a message](https://reddit.com/message/compose/?to=paw_tipbot&subject=command&message=create) to /u/paw_tipbot.
Once you have funds in your account, you can tip other redditors, or send to any PAW address via PM to /u/paw_tipbot.
# Comment Replies:
PAW Tipper is intended for tipping on reddit posts and replies.

On supported subreddits, you can send a tip like this:

    !paw 1 This is great!

This will tip a redditor 1 PAW and send "This is great!" along with your Reddit username as a tip note. !paw <amount> must be the first thing in your message OR the last thing. Such, this is also a valid tip, but will not send a tip note:

    This is great! !ban 1

Or from anywhere on reddit, you can tip a commenter by:

    /u/paw_tipbot 1 This is great!
   
or

    This is great! /u/paw_tipbot 1

If the subreddit is a friendly subreddi, the bot will repsond with a message. If the subreddit is not friendly, a PM will be sent to both the sender and the recipient.
    
# Private Messages

Banano Tipper also works by PM. [Send a message](https://reddit.com/message/compose/?to=paw_tipbot&subject=command&message=type_command_here) to /u/banano_tipbot for a variety of actions.

To send 1 PAW to u/ApolloRiver, include this text in the message body:

    send 1 /u/ApolloRiver
-or-

    send 1 ApolloRiver

To send 1 PAW to paw\_3rqguc66m3b7s1zuq1fzyqdyx94hzeydczekc6zk9i7w88i3n4wuco7jxrss, include this text in the message body:

    send 1 paw_3rqguc66m3b7s1zuq1fzyqdyx94hzeydczekc6zk9i7w88i3n4wuco7jxrss

or send all your balance:

    send all paw_3rqguc66m3b7s1zuq1fzyqdyx94hzeydczekc6zk9i7w88i3n4wuco7jxrss

There are many other commands.

```
'balance' or 'address' - Retrieve your account balance.
'create' - Create a new account if one does not exist
'help' - Get this help message
'history <optional: number of records>' - Retrieves tipbot commands. Default 10, maximum is 50.
'send <amount or all, optional: Currency> <user/address>' - Send PAW to a reddit user or an address
'silence <yes/no>' - (default 'no') Prevents the bot from sending you tip notifications or tagging in posts
'subreddit <subreddit> <'activate'/'deactivate'> <option>' - Subreddit Moderator Controls - Enabled Tipping on Your Sub (`silent`, `minimal`, `full`)
'withdraw <amount or all> <user/address>' - Same as send
'opt-out' - Disables your account.
'opt-in' - Re-enables your account.
```
### Control TipBot Behavior On Your Subreddit
If you are a moderator of a subreddit, and would like to tipping to your sub, use the `subreddit` command. For example, for me to activate tipping on my /r/banano_tipbot subreddit, I send a PM to the bot saying:

`subreddit paw_tipbot activate`

This will allow the bot to look for !ban commands and respond to posts. 
-or- If I don't want the bot to respond, but still want tips:

`subreddit paw_tipbot activate silent`

-or- for a cleaner tipbot response:

`subreddit paw_tipbot activate minimal`

To deactivate, simply PM

`subreddit paw_tipbot deactivate`

### Here's a few other great links:
[Banano Subreddit](https://reddit.com/r/paw_digital) -- Post any questions about Banano Tipper
[Banano Tipper GitHub](https://github.com/SecureChainFinance/paw_reddit_tipbot) -- This software is open source!
[BANANO](https://paw.digital) -- The Official PAW website
[Biome](https://wallet.paw.digiral) -- The Official PAW Web Wallet

# Terms of Service
* Don't keep a lot of PAW in your Tip Bot account!
* You accept the risks of using this Tip Bot--We won't steal your PAW, but they might be lost at any point, and we are at no obligation to replace them. Don't put in more than you're willing to lose.
* If your account is inactive for more than 3 years, and no meaningful attempt has been made to reach me, the PAW in your account are subject to be forfeited and we are under no obligation to return them. The tip bot is not a lifelong custodial service.
* Don't submit more than 5 requests every 30 seconds. The bot will ignore any commands you issue until 30 seconds have passed.
* I can change the Terms of Service at any time.

# FAQ
## Why does the message have to start or end with !paw <amount>?
This is to prevent unintentional tips! If the program simply scanned the entire comment, a user might accidentally quote someone else's tip command in a response. In the future I might change this, but for now it's the best way to ensure the program behaves as expected.

## Are my funds safe?
**NO! Unless you and you alone control your private keys, your funds are never safe!** Please don't keep more than a small amount of PAW on the tipbot at any time! While I'm not going to steal your PAW, this program is in early beta testing and weird things could happen, including lost PAW! **Use at your own risk!** (sorry for all the exclamation marks)

## I sent a tip to the wrong address. Can I get it back?
If the address isn't affiliated with a Redditor, **No.** We only have private keys for redditors, not for external addresses.

## I sent a tip to the wrong redditor. Can I get it back?
Your best bet is to try to reach out to the redditor and ask for it back. Do not harass other redditors or do anything that would violate Reddit's Terms of Service.

## Have you implemented any spam prevention for your bot?
Users are allowed 5 requests every 30 seconds. If you do more than that, the bot ignores you until 30 seconds have passed.

## I tried to send a tip, but received no response. Did it go through?
Probably not. It's most likely the bot was temporarily disconnected. If a command is issued while the bot is offline, the command will not be seen. If no response is received from the bot after a few minutes, send a message to the bot with the text 'history'. If you get a response and the tip isn't in your history, that means it wasn't seen. If you don't get a response, the bot is probably still offline. Try again in a few minutes.

## I found a bug or I have a concern. Question Mark?
Post on the [PAW subreddit](https://reddit.com/r/paw_digital) or reach on on the [Discord (https://discord.com/invite/DjXn6bb3aE)

# Error Codes
If a reddit tip is a reply to a reply, it's better to keep a short message with an error code.
* 100 - You do not have an account -- Create an account by typing 'create' or by receiving a tip from another redditor.
* 110 - You must specify an amount and a user, e.g. `send 1 paw_tipbot`.
* 120 - Could not read the tip amount -- use either a number or the word 'all'.
* 130 - Tip amount is below program minimum -- This is to prevent spamming other redditors.
* 150 - This subreddit does not accept tips this small, increase your tip or send the bot `subreddit subreddit_name` to see what the minimum is.
* 160 - You have insufficient funds.
* 190 - The recipient has disabled tipping for their account.
* 200 - You have tried to tip your own comment or withdraw to your own account, which is not allowed.
