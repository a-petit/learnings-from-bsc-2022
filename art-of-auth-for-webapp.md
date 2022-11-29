# Art of auth for webapp


When it comes to realize auth, we all follow the same path:
- search on web
- do the rest of fucking stuff
- Nobody understand what he is doing

Nick craver tweet auth code

## Intro to standards

- Digital identity : set of attributes that define user
- Authentication : prove who you are
- Authorization : grant access

## Oauth 2.0
What problem it solve ? 
- Before : when using app that use for you on bewalf, need to share credentials. 
- Baaaad ! + way too much access

Open standards for performing delegated authorization.
Authorization server : provide endpoints , generate tokens

Oauth encoutered great success.

Confused Deputy problem : oauth purpose handle Authorization but not authentication.

Oauth : delegated autho
Openid connect : authentication

Id tokens
Access tokens

Slides on linktr.ee/kimmaida

Json web token
header
content
signature : so it can’t be modified

Only server can decrypt and sign tokens

Use services to validate signatures and don’t do it manually.

Access token often use jwt but it’s not necessary. They are opaque to client. Scope is a subset of user’s permissions

Putting all things together
Design caps
Do stickers and distribute them . Give people a reason to come and talk with you

Cookie can be used to store the token. No cookie or expired ? 302.

Don’t put tokens in local storage - especially if they are long lived

Refresh token ok.
Cookie = ok if a single domain.
SpA + single dimain : cookie ok
Spa + multiple domains : token

PKSE

Identity = big subject
m’aida.kim, linkedin