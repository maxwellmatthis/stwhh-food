# stwhh-food

**This project is in its networking phase. Please share links to this README with other software nerds to increase reach and intelligence!** Remember to star the repo or check back soon for changes. Don't hesitate to send me an email if you have further thoughts or just want to be reminded if something happens.

## Description

A crawler that feeds a server that helps aggregate and track food offerings for the cafeterias and cafes operated by Hamburgs student works.

## Background

The [food website of Hamburg's student works](https://www.stwhh.de/speiseplan?t=this_week) isn't perfect. It's slow, there's a lot of text boiler plate and scrolling, its filters don't have much variety and are sometimes broken, it doesn't track interesting statistics, there is not official app, the only way to get notifications is getting the whole weeks schedule via email, etc. ([Add your wishes here](#wishes)) Unsurprisingly with so many computer scientists and engineers there are [a hand full of projects](#other-solutions-attempting-to-improve-food-finding-efforts) that have started working on better tools. But it's the most complete and well maintained project I can find.

So here I am setting out to create yet another project. Hopefully we can get a **larger group of software nerds** to work on this together **to make a tool** that **people will actually use**. Maybe the project can graduate from the TUHH and become known across Hamburg.

I'm explicitly starting this project, not by coding, but by creating this README to kickstart the networking and intelligence gathering process. Coding a first MVP should be fairly straight forward, but some planning is probably a good idea and maybe we _won't even have to create anything new_, if there is already an app that meets our [requirements](#wishes).

## Wishes

If you have any pain points concerning the cafeterias or cafes of the STWHH, please think of what feature or property would solve that problem and add it to the list via pull-request:

_A better stwhh food application should be/should have..._

- very fast
- mobile first but powerful on desktop too
- most relevant information within one screen at the top of the page to prevent having to scroll
- information about opening/closing times
- information about allergies
- information about sustainability
- realtime crowd-sources data (which meals are sold out, is there still fruit, is there desert, is there a long line)
- statistics (frequency/pattern of specific meals, prices)
- a webapp
- a GraphQL API to make coding the frontend and third party apps easier
- hosted by the university (AStA or an FSR) long term

If your wish collides with someone else's wish, please still add it and do not remove the other person's wish. You can also enhance someone else's wish by adding further information behind it in parenthesis (`(...)`).

## Other solutions attempting to improve food finding efforts

**Please help maintain the list below**, so that we can finally bundle our efforts and learn from mistakes and not keep creating new food tracking software in Hamburg:

- [stwhh-mensa](https://github.com/pixlcrashr/stwhh-mensa) - As of April 2026, an unfinished, unmaintained project written in go that crawls the website and saves details for aggregation purposes. There isn't very much documentation and significant time seems to have been spent on database schemas and making the software runnable via docker. Also there isn't a webpage or an API yet, so the project isn't very far along on the way to reaching it's MVP in my opinion.
- [TUHH-Mensa](https://github.com/Lukas-Fohl/TUHH-Mensa) - A small command line utility that gets the names and prices of food and sends them to the push service ntfy.sh. The project seems alive but very small and lacks the ambition to be a fast, customizable tool with high information density. I will try to join forces with the creators.
- [Mensaplan](https://www.mensaplan.de/hamburg/mensa-harburg/index.html) - A fairly mature piece of software that is closed source, run by an advertising company and not very optimized for Hamburg, which means that it doesn't show allergy information and so on.

## Project Vision (technical)

- As little overhead (i.e. frameworks, hyperscaling readyness) as possible until the project actually needs it.
- Two - either python or go (because of simplicity) - based applications;
    - one that crawls and can be triggered by a scheduler such as cron, and
    - one that provides a webserver and graphQL API.
- One minimal PWA (web app) for now that gets data based on customization options.

## Tags to help other find this project

As always feel free to contribute:

- Studierendenwerk Hamburg Mensa
- Essen Mensa Hamburg
- Mensa TUHH
- STWHH Mensa
- STWHH TUHH
- Technische Universität Hamburg Mensa
- STWHH Cafe
