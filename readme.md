# SelfHost_DataStoreService
A self-hosted datastore service for roblox development, with two modes: Drop in replacement, and Secured.

## Drop in
This would be an exact drop in replacement. All you need is to import the api and to transfer data. 

## Secured
Secured is a more secure implementation. You'd want to use this in more secure contexts, and/or contexts when you'd only be accessing during certain events, you would not store rapid changing player data here! For example, when storing feature flags or admin lists. 
You'd also want to use this in cases where other outside programs would access the data, ex: a discord bot. 

`This is neither meant for rapid changing data nor is it a drop in replacement.`

This uses
 - E2EE
 - Salting based on Creator Id
 - Seperate Decryption  