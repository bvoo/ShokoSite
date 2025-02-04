+++
title = "Shoko Version 4.2.0 Released"
image = "assets/images/blog/Version-420-Banner.jpg"
date = 2023-03-20T09:16:46-07:00
type = "post"
anime = "Handyman Saitou in Another World"
category = ["Update"]
tag = ["Shoko Server", "Shoko Desktop", "Shokofin"]
dev= ["Avael", "Baine", "Cazzar", "Da3dsoul", "fearnlj01", "krbrs", "Mik1ll", "Mohan226", "Revam"]
+++

We are thrilled to announce the release of the latest version of Shoko! This new version introduces numerous
enhancements, novel features, and bug fixes that improve the user experience significantly.

For a comprehensive list of changes, kindly visit our [Changelog](https://docs.shokoanime.com/changelog/).

##### Basic ARM64 Support

Thanks to **Mohan226**, we're now able to offer an ARM64 build of Shoko on Linux

However, please note that all initial testing was conducted in a virtual machine. As there are numerous devices
running on ARM64, we will not provide support for getting Shoko to work on your device. Although you can always ask,
as this is an uncharted territory, we'll depend on users to document the path forward.

Please keep in mind that several ARM devices do not meet the minimum requirements of Shoko. In case it runs, it will
perform exceptionally poorly and might even crash. We do not intend to optimize for these kinds of devices. 

We're looking into getting an ARM64 build of Shoko working on Mac and hope to have something available soon for users 
to test out. 

##### Final Minor Release

This minor release marks the conclusion of version 4 as we prepare for the next major release, version 5. Although
we are not yet prepared to disclose what to expect, as there are still many aspects to work out, we can say that
this is something the team, particularly **da3dsoul**, has been eager to do for a very long time. We will probably
post a future blog detailing the changes since we anticipate a prolonged beta period when these changes are made.
However, let's just say goodbye to nHibernate.

**Due to the database changes, the latest 4.2.X version will be required to upgrade to Shoko 5.X.X once release.**

##### .NET 6 and AniDB Rewrite Brings Speed and Bug Fixes

The transition to .NET 6 and the comprehensive rewrite of the AniDB provider were two significant impediments that
contributed to the extended period between releases. However, despite the fact that both of these significant
changes are not visible to the end-users, they still offer tremendous benefits. The shift to .NET 6 provides better
compatibility, performance enhancements, and establishes the framework for future changes that we intend to make to
Shoko. The AniDB rewrite addresses several bugs and unforeseen issues with AniDB as a provider while significantly
increasing speed.

##### Major SQLite Work

Significant effort and time were invested in improving overall performance when using SQLite as your database. Since
making SQLite the default database type for Shoko, we've been working on improving the user experience and making it
comparable to users on legacy database types such as MySQL or SQL Server. With our SQLite system finally supporting
WAL (Write-Ahead-Logging), users should notice a significant improvement in startup times and response. It has also
helped to reduce the dreaded database lock errors that frequently appeared. Additional work was also done to address the
remaining database lock errors. Although we've done extensive testing, please keep an eye out and report any database
lock errors you see in your log.

##### Shokofin 3.0.0

The latest update to Shokofin has introduced several exciting new features and improvements. Users can now finally
synchronize watch states between Shoko and Jellyfin, including the ability to import, export, and sync watch states
outside the live-scrobbling feature. Furthermore, the update adds support for parental ratings for H content, enabling
users to skip syncing such content if desired. Parental rating for other content will be introduced in another update
later.

Other fixes and improvements include better handling of multi-series files, ensuring that file locations match between
client and server environments, and fixing issues related to specials placement and episode titles for some OVAs.
Furthermore, the scrobbler has been updated to scrobble less often, resulting in less spam in the log.

For users who enjoy experimenting with new features, the update introduces an experimental section in the plugin
settings that enables them to toggle new, mostly untested features. These include the ability to merge multiple versions
of episodes in your Shoko managed library, as well as changing to the experimental chronological season sorting.

##### Enough Reading, Get Shoko 4.2.0 Now

To download the latest release and view the detailed changelog, head over to
our [Downloads Page](https://shokoanime.com/downloads/).

We hope you enjoy the new features and improvements in this release. As always, we appreciate your feedback and support.
Happy organizing!

##### Contributors

This release was made possible by the following people.