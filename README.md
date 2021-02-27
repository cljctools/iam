# iam
a library to handle user sing-in, identity etc. in an app

## rationale

- stemming from 
  - https://github.com/DeathStarGame/DeathStarGame/issues/41#issuecomment-787013446
  - https://github.com/sergeiudris/deathstar.lab/blob/5ded13005e37d553ebba87dd7429d30c211681bd/docs/search-for-the-game.md
- reusable: when building our app, we want everything-identity to be a reusalbe 'plugin'/layer/lib
- similar for example to how https://github.com/metosin/reitit solves http service with multiple choice of servers, async librarries etc.
- db of choice: have a transport/adapter for that db (adapter is a list of fns for read and write IAM ops, translates how to put/retrieve that data to/from db of choice)
- http server of choice: we want to use reitit at least
