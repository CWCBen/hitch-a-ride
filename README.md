# Hitch-a-Ride
Mobile app for EECS 441 by Brian Ford, Jon Budzenski, and Madi Sergazin.

## Prereqs
Node.js and npm.

## Setting up Development Environment

Fork this repo, and the following three:
* [client](https://github.com/btford/hitch-a-ride-client)
* [server](https://github.com/btford/hitch-a-ride-server)
* [android](https://github.com/btford/hitch-a-ride-android)

Then clone the following repos, replacing `btford` with your user name:
```
git clone git@github.com:btford/hitch-a-ride.git
git clone git@github.com:btford/hitch-a-ride-android.git
git clone git@github.com:btford/hitch-a-ride-server.git
git clone git@github.com:btford/hitch-a-ride-client.git
```

[`npm link`](https://npmjs.org/doc/link.html) client, server, and android:
```
cd hitch-a-ride-client && npm link
cd ../
cd hitch-a-ride-server && npm link hitch-a-ride-client && npm link
cd ../
cd hitch-a-ride-android && npm link hitch-a-ride-client && npm link
cd ../
cd hitch-a-ride && npm link hitch-a-ride-server && npm link hitch-a-ride-android
```

Now changes you make in each repo will be reflected in all of the repos that depend on it.


## License
MIT
