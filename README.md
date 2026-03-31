# Gmail Drain

Simple script to remove emails from gmail, since they make it hard.

> [!CAUTION]
> No effort is made to protect yo creds.
> Blame google's ai slop sample code.

## Setup
Create a google developer app. Get your client info, put it in the credentials.json file.

## Usage

Just supply any query as argv[1]. Essentially, any search query you can put in the search bar, you can use here.

> [!WARNING]
> You will not be prompted for confirmation.
> You will not see a pretty list.
> Things will simply go into the forever box

```bash
# Purge a domain
python3 ./main.py 'from:discord.com'

# Maybe anything from before 2020
python3 ./main.py 'before:2020'

# Anything from riot that isn't a receipt
python3 ./main.py 'subject:-Receipt from:riotgames.com'
```
