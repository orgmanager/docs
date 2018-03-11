---
title: Frequently Asked Questions
---

## Why does OrgManager need admin access to my organization?

The GitHub API (the way third-party applications like OrgManager interact with GitHub) requires admin permissions to invite users to the organization. Think about it! if we allowed anyone, every user of your organization could invite anyone! Seems a bit risky...
Anyway, if you still don't trust us, OrgManager is open-source, so you (or your developer team) can have a look at the code and tweak it.

## My organizations aren't showing in the dashboard

First, verify you have authorized OrgManager to access your organization. You can do that by accessing the [OrgManager permssions page](https://github.com/settings/connections/applications/10b01d866046f040c9f1) at GitHub, and verifying that a green tick is showing next to the organization name. If it isn't, click the "Authorize" button, and if nothing of this worked or you can't find the button, [open an issue](https://github.com/orgmanager/orgmanager/issues/new?title=Can%27t%20authorize%20OrgManager&body=Please%20explain%20your%20issue%20details%20here%20and,%20if%20possible,%20add%20an%20screenshot).
Once you verified OrgManager has access to your organization, [sync again](https://orgmanager.miguelpiedrafita.com/sync).

## How can I get in contact with the OrgManager team?

Read the [OrgManager Support Channels](doc:orgmanager-support-channels) page.

## Why don't you have a domain name for OrgManager?

I believe the budget for open-source projects should be $0, and since I started OrgManager, I haven't spent anything besides the hosting. If you would like to donate, head over to our [OpenCollective](https://opencollective.com/orgmanager) page.