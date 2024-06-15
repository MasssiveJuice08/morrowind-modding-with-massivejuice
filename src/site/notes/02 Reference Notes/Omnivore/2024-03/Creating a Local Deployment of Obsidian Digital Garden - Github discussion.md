---
{"dg-publish":true,"permalink":"/02-reference-notes/omnivore/2024-03/creating-a-local-deployment-of-obsidian-digital-garden-github-discussion/","title":"Creating a Local Deployment of Obsidian Digital Garden - Github discussion\n","metatags":{"description":"Github discussion demonstrating how to set up a local deployment of Obsidian Digital Garden","og:image":"https://i.imgur.com/LmCg5HX.png"},"tags":["obsidian-digital-garden"]}
---


## About

#Omnivore

[Read on Omnivore](https://omnivore.app/me/local-deployment-oleeskild-obsidian-digital-garden-discussion-16-18e501c54ac)
[Read Original](https://github.com/oleeskild/obsidian-digital-garden/discussions/160)

Github discussion demonstrating how to set up a local deployment of Obsidian Digital Garden

_This page is powered by [Omnivore](https://omnivore.app) ‐ you can read more about how I use Omnivore here: [[02 Reference Notes/Omnivore/Omnivore - Saving Articles for Citations in Obsidian\|Omnivore - Saving Articles for Citations in Obsidian]]._

### Highlights

> I threw something together you could use to run this locally:
> 
> 1. Clone your digital garden repo to your computer
> 2. run `npm install express --save` to install express as a dependency.
> 3. Create a new file in the root folder called app.js, and paste the following code:
> 
> const express = require('express')
> const app = express()
> const port = 8080; 
> 
> const searchHandler = require('./netlify/functions/search/search.js').handler;
> 
> app.get('/api/search', async (req, res) => {
>   //Mock the netlify event
>   let event = {queryStringParameters: req.query};
> 
>   let response = await searchHandler(event);
>   res.status(response.statusCode).send(response.body);
> })
> 
> app.use(express.static('dist'))
> 
> app.get('*', (req, res)=>{
>   res.redirect("/404")
> })
> 
> app.listen(port, () => {
>   console.log(`Digital garden running on port ${port}`)
> })
> 
> 1. Run `npm install`
> 2. Run `npm run build`
> 3. Run `node app.js`
> 
> The site should now be available at localhost:8080.
> 
> You can then use something like [pm2](https://pm2.keymetrics.io/) to run it on your server, and use a r[everse nginx proxy with lets encrypt](https://seanthegeek.net/1035/how-to-configure-a-nginx-reverse-proxy-with-lets-encrypt-certificates/) to expose it on port 443 with https. [⤴️](https://omnivore.app/me/local-deployment-oleeskild-obsidian-digital-garden-discussion-16-18e501c54ac#9d0353fc-b12c-4dfc-acdf-e900471a781a) 
{ #9d0353fc}


Method for creating a local deployment of #obsidian-digital-garden

