
# doodle-cli - Create doodle polls from the commandline #

A scriptable way to create doodle polls.

## Installing ##

Requirements:

- python 2 >= 2.6
- requests-oauthlib 
- everything else is in the standard library

Clone this repo and then install requests_oauthlib

    pip install requests_oauthlib

## Running ##

1 Register for doodle.com
1 Get yourself a consumer key and secret from https://doodle.com/mydoodle/consumer/credentials.html
1 Set the consumer key and secret as environment variables:
    export DOODLE_CONSUMER_KEY='whatever'
    export DOODLE_CONSUMER_SECRET='something'
1 Create a poll
    $ create-doodle-poll -t 'My poll' -d "The teddy bears' picnic" \
       -i graham@example.com -n 'Graham' -p 'Attending' -p 'Not attending'
    http://doodle.com/polls/vyu3hxq9u4qpnqn6
