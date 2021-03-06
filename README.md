#Why this fork?#
It's not final, I just wanted to have a script which notifies me about a new Pokemon around my position. You know, you're at work and you don't want to turn the app every minute just to check if there's a new Pokemon.
I hope I'll make some cleanup after it's functional, maybe I won't need the map itself. This is the purpose of original PokemonGo-Map application and I don't intend to duplicate it, I just wanted to start with some functional code as soon as possible.

## Possible usage#
This is how I use it now (change IP addresses and credentials to your own). You need to get your user/password at https://www.pokemon.com

<b>Output to file</b>

./example.py -H 127.0.1.1 -u user -p password -l "Google Maps location" -st 1 2>/dev/null >>/tmp/output.log

Or simply use it without redirecting

<b>Parse and stream file</b>

ncat -lk 5566 -c 'tail -f /tmp/output.log'

<b>Read data remotely</b>

nc -v 127.0.0.1 5566

#Support for master branch dropped.#
##Accepting only pull requests for develop branch. ##

#[Official Website] (https://jz6.github.io/PoGoMap/)#

##[Android Port](https://github.com/omkarmoghe/Pokemap) <== Direct all andriod related PRs and discussion here.

Please submit all pull requests to [Develop Branch](https://github.com/AHAAAAAAA/PokemonGo-Map/tree/develop)

<p align="center">
<img src="https://raw.githubusercontent.com/AHAAAAAAA/PokemonGo-Map/master/static/cover.png">
</p>

# PokemonGo Map

[![Build Status](https://travis-ci.org/AHAAAAAAA/PokemonGo-Map.svg?branch=master)](https://travis-ci.org/AHAAAAAAA/PokemonGo-Map) [![Coverage Status](https://coveralls.io/repos/github/AHAAAAAAA/PokemonGo-Map/badge.svg?branch=master)](https://coveralls.io/github/AHAAAAAAA/PokemonGo-Map?branch=master)

Live visualization of all pokemon (with option to show gyms and pokestops) in your area. This is a proof of concept that we can load all nearby pokemon given a location. Currently runs on a Flask server displaying a Google Map with markers on it.

Using this software is against the ToS and can get you banned. Use at your own risk.

Building off [Mila432](https://github.com/Mila432/Pokemon_Go_API)'s PokemonGo API, [tejado's additions](https://github.com/tejado/pokemongo-api-demo), [leegao's additions](https://github.com/leegao/pokemongo-api-demo/tree/simulation) and [Flask-GoogleMaps](https://github.com/rochacbruno/Flask-GoogleMaps).

---
#For instructions, please refer to [the wiki](https://github.com/AHAAAAAAA/PokemonGo-Map/wiki)#

Hello Paul Xu the Internship king ;)
