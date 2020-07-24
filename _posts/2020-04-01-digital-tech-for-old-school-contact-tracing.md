---
layout: post
title:  "Digital tech for old school contact tracing"
date:   2020-04-01 23:22:40 +0000
---

Contact tracing is a central tool in the fight against the epidemic. However, it is a laborious and time-consuming task, which limits its usefullness.

Ideally, everyone would keep a record of the people they were in contact with, so that when someone is confirmed positive, his/hers close contacts for the last few weeks are quickly identified and tested, hopefully containing the chain of transmission. In reality, people's memories are not perfect, and authorities need to resort to additional means to identify potential infections. 

As [IGC](http://gulbenkian.pt/ciencia) was planning its reopening post-confinement, scientists and staff were encouraged to keep a contact log. To facilitate this, we developed a web app that enables quick and private contact logging. It is unimaginatively called [ *ContactLog* ](https://igc-qds.github.io/contactlog/). 

*ContactLog* makes use of progressive web technologies to deliver a smooth and private experience. It saves all the data locally on your browser (using `localStorage`) and nothing gets communicated to a server (there is no server, beyond the instalation). It uses `serviceWorkers` to download all the files it needs to function, so that it works even if you have no internet access. 

Source code is [here](https://igc-qds.github.com/contactlog) and the deployed version is [here](https://igc-qds.github.io/contactlog/).