---
layout: post
title: "Add gem owner add and remove in web UI of rubygems.org"
image: '/assets/img/'
main-class: 'rubygems'
tags:
- rubygems
- rubygems.org
- rails
introduction: 'We will add options for adding/removing gem owners via Web UI. Additionally, we will make owner add/remove events notifiable. We will also add a new flow for ownership transfers.'
---

`gem owner -a/r` [command](https://guides.rubygems.org/command-reference/#gem-owner) is used to add or remove owners by an email. This method requires that the user has the `gem` CLI configures on a host.
Option of adding and removing owners through the web UI would facilitate friction-less transfer of gem ownership. To avoid spamming, adding a new owner would require a confirmation from the user being added. We will update the existing [`POST - /api/v1/gems/[GEM NAME]/owners`](https://guides.rubygems.org/rubygems-org-api/) to follow the same process where a confirmation is required. Additionally,
We will make owner add/remove events notifiable, ie users can opt-in to receive email notification about ownership changes of a gem.

We are also hoping to add a new flow for ownership transfers, where users can make `ownership request` for any gem with less than 100_000 downloads and older than 12 months updated at time. When a gem owner approves an ownership request, the requester would be added as an owner to the gem. Gem owners who are looking for new maintainers/owners would be able to request `ownership application`. These application will be searchable and listed on a site wide link.

* **Related**: [#2044](https://github.com/rubygems/rubygems.org/issues/2044), [#725](https://github.com/rubygems/rubygems.org/issues/725), [#1842](https://github.com/rubygems/rubygems.org/pull/1842)
* **Prerequisites**: Familiarity with rails
* **Programming areas include**: ruby, rails
* **Estimated difficulty level**: medium
* **Student**: Pavan Vachhani
* **Mentors**: @sonalkr132

## Status Updates

### Week 3 (06/19/2020)

1. What did you accomplish this past week?
    - (add your accomplishments)

1. What will you do this upcoming week?
    - (add your tasks for next week)

1. What obstacles are impeding your progress?
    - (list any obstacles)

1. Would you like help from some mentor for this task?
    - (list any help you need)