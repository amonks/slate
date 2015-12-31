# Server

## current responsibilities

1. provide the client with gifs
2. *handle* social stuff

## current endpoints

verb | endpoint | description
---- | -------- | -----------
`get` | /share/facebook | redirect to /connect/facebook, which then redirects to /facebook/callback
`get` | /facebook/callback
`get` | /share/twitter
`get` | /twitter/callback
`get` | / | redirect to client
`post` | /share/email | email gifs using mandrill
`post` | /share/instagram
`post` | /share/mms
`get` | /tweets
`get` | /tweets/:max_id | get tweets before :max_id
`get` | /tweet/:tweet_id
`get` | /incoming/:tweet_id | get `gif-ready` notifications from the booth
`get` | /flush | flush cache

