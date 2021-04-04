---
title: How I Organize My Rails Apps
date: 2015-01-22
tags: rails
---

In this blog post I explain how I organize my Rails apps.

READMORE

If you know Rails, then you already probably know about the following:

## app

- `app/models` for ActiveRecord and non-ActiveRecord models
- `app/models/concerns` for model concerns
- `app/controllers` for Rails controllers
- `app/controllers/concerns` for controller concerns
- `app/assets/javascripts` for javascript assets
- `app/assets/stylesheets` for stylesheet assets
- `app/assets/images` for images
- `app/views` for all view templates
- `app/workers` or `app/jobs` for workers/jobs

If there are multiple objects in the `app/models` folder that seem to follow a pattern, like `PaymentNotification`, `OrderNotification`, then you can move those into its own folder: `app/notifications`

## lib

The typical situation is that files that don't seem to fit anywhere then are dumped into `lib`. The problem with this is that it gets bloated. What I've found helpful are the following:

- `app/services` for service objects that **are verbs**, like:
  - `ProcessCreditCard`
  - `BroadcastPaymentNotification`

Only classes that are not specific to my application go to the `lib` folder. These classes may be used in other projects -- perhaps you have the intention of making a gem from them.

## vendor

- `vendor` for third-party libraries that are not installed via a gem for some reason.

## Assets

When it comes to assets, I have the same rules of thumb as above:

- `app/assets` for assets that are specific to my application
- `lib/assets` for assets that I have that may be used in other apps
- `vendor/assets` for third party assets that are not installed via gems

There's one difference: when a asset "package" asset is neither pure JS or pure CSS, then I create a `plugins` folder under `assets`. For example: `vendor/assets/plugins/carousel-4.2.1`

## Specs

My spec files are organized the following way:

- `spec/models`
- `spec/controllers`
- `spec/workers`
- `spec/jobs`
- `spec/services`
- `spec/lib/some_library_that_i_made`

In short, anything that is in `app` gets it own folder directly under `spec`. If I'm testing something in `lib`, then I create a `spec/lib` folder and put the specs in there.

There are other things to cover like custom RSpec matchers but they are RSpec specific. I may talk about them in a different post.
