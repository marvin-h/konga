# Change Log

All notable changes to this project will be documented in this file.

## [0.10.2](https://github.com/pantsel/konga/releases/tag/0.10.2) - 01-03-2018

* **[Fix]** Fix issue [#178](https://github.com/pantsel/konga/issues/178) that produced hook timeouts.
* **[Fix]** Fix issue [#175](https://github.com/pantsel/konga/issues/175). Health checks are now removed when an API is deleted.
* **[Fix]** Fix GET targets AND Add possibility to select Hash_on for Upstreams for Kong 0.12.x.
* **[Fix]** Fix SSL connection to Postgres.
* **[Fix]** Fix api timeouts to match Kong defaults.
* **[Enhancement]** Feature to change Konga default users [#168](https://github.com/pantsel/konga/issues/168).
[See details](https://github.com/pantsel/konga/blob/master/DEFAULTUSERSEEDDATA.md)
* Various other minor bug fixes and improvements.

#### Breaking Changes
Since the upstream targets GET call is changed to match Kong's 0.12.x changes, it will not
work on previous Kong versions



## [0.9.1](https://github.com/pantsel/konga/releases/tag/0.9.1) - 06-12-2017

* **[Fix]** Fix certificate uploads.
* **[Enhancement]** Reveal all of oauth credential info in consumer credentials list.
* **[Fix]** Address connection ui issues.
* **[Fix]** Fix user signup.
* **[Enhancement]** [Add environment variables for socket adapter configuration to allow easy socket configuration in docker.](Add environment variables for socket adapter configuration to allow easy socket configuration in docker.)


## [0.9.0](https://github.com/pantsel/konga/releases/tag/0.9.0) - 23-10-2017

> A database update is required! Make sure you run Konga in dev mode once so that
the migrations will take place.

* **[Enhancement]** Only admin users can access snapshots.
* **[Enhancement]** You don't have to manually specify Kong version when creating a connection anymore. It is now retrieved automatically throughout the application.
* **[Enhancement]** You can now schedule your Kong node snapshots and leave Konga to do the rest. 
* **[Enhancement]** Introducing connection types (**Breaking change**). 
* **[Enhancement]** Added support for `JWT Auth Loopback API`. 
* **[Fix]** Fixed some issues with snapshots and snapshot restoration.
* **[Fix]** Consumer imports are working again.
* **[Fix]** Fixed database info display on dashboard page when using Cassandra.


#### Breaking Changes
Due to the new **Connection types** logic, the existing connections to Kong admin
API are likely to stop working. You will need to create new ones using the new forms.
No data or settings will be lost.

## [0.8.9](https://github.com/pantsel/konga/releases/tag/0.8.9) - 8-10-2017
* Allow certificates deletion.
* Manage SNIs from certificates detail modal.

## [0.8.8](https://github.com/pantsel/konga/releases/tag/0.8.8) - 8-10-2017

* When starting the app for the first time using postgres or MySQL adapters, Konga will now create the databases automatically.
* Parts of UI are redesigned in a cleaner way.
* Consumer page now also displays the APIs a consumer can access based on his ACLs.
* Slack integration. You can now configure Konga to send notifications to slack.
* Fix issue which prevented consumer creation with empty `username` or `custom_id`.
* Other minor bug fixes and improvements.

## [0.8.0](https://github.com/pantsel/konga/releases/tag/v0.8.0) - 23-5-2017

* UI/UX revamp.
* Massive refactoring and logic improvements.
* Configurable user permissions.
* Various bug fixes and improvements.

## [0.8.7](https://github.com/pantsel/konga/releases/tag/0.8.7) - 29-9-2017

* [FIX] Tests are working again.
* [FIX] Better error handling when adding groups and credentials to consumers.
* [FIX] <code>kongadata</code> dir is now created inside the project folder by default. The docker volume now becomes <code>/app/kongadata</code>

## [0.8.6](https://github.com/pantsel/konga/releases/tag/v0.8.6) - 24-9-2017

## [0.8.5](https://github.com/pantsel/konga/releases/tag/v0.8.5) - 23-9-2017

* Fix docker automated builds failure.
* Removed kong admin url from connections chooser.
* Sails js hookTimeout is now configurable via env var <code>KONGA_HOOK_TIMEOUT</code>.

## [0.8.4](https://github.com/pantsel/konga/releases/tag/v0.8.4) - 19-9-2017

* Fix bug where a new user could not be created when users where not allowed to sign up.
* Hide API keys in connections when logged in as a simple user.

## [0.8.3](https://github.com/pantsel/konga/releases/tag/v0.8.2) - 20-8-2017

* Kong 0.11.x compatibility.
* Added the ability to manage consumer plugins directly from the consumer edit page.
* More dynamic backwards compatibility logic.
* Other minor fixes and improvements.


## [0.8.1](https://github.com/pantsel/konga/releases/tag/v0.8.1) - 3-7-2017




 






