## Start a local Solid Server with demo data

```
npm ci
npm start
```

## Accessing the local server

The server will be running at [http://localhost:1526](http://localhost:1526). There is a pre-configured Pod for demo user `alice` at [http://localhost:1526/alice/](http://localhost:1526/alice/)

Access the Pod using PodOS Browser at [https://browser.pod-os.org/?uri=http%3A%2F%2Flocalhost%3A1526%2Falice%2F](https://browser.pod-os.org/?uri=http%3A%2F%2Flocalhost%3A1526%2Falice%2F)

## Demo credentials

Sign in using:

Identity Provider: http://localhost:1526/  
Email: `alice@sosy26.example`  
Password: `alice`  

## Exercise

Alice has built an [inventory](https://browser.pod-os.org/?uri=http%3A%2F%2Flocalhost%3A1526%2Falice%2Finventory) from the things she [ordered](https://browser.pod-os.org/?uri=http%3A%2F%2Flocalhost%3A1526%2Falice%2Forders%2F), but she lent some of her things to her [friends](http://localhost:1526/alice/my-contacts/people.ttl). She wants to keep track of what she gave to whom.

1. Create a new container for `lendings` using [PodOS Browser](https://browser.pod-os.org)
2. Create a new [schema:LendAction](https://schema.org/LendAction) using "Add new thing"
3. Add `startDate`, `borrower` and `object` using "Add literal" and "Add relation" in the "Data" tool
4. [Build a dashboard](https://pod-os.org/getting-started/quick-start/) showing all lendings using PodOS elements