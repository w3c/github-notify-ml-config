W3C configuration for *github-notify-ml*: send e-mail to individuals or mailing lists when events happen to /TR specs or GH repositories.

Please refer to the project [github-notify-ml](https://github.com/dontcallmedom/github-notify-ml/) for information.

## W3C instance
W3C operates an instance of github-notify-ml service for WGs (and some CGs) repositories; if you want to make use of this service, please send pull requests on this repository with amendments to the <code>mls.json</code> file for the mailing list(s) and repo(s) you’re interested in.

All repositories in the `w3c` organization are set up to make use of the notification service by default; if you want to use it for a non `w3c/` repository, you will need to add a webhook to https://services.w3.org/github-notify-ml/ in the target repository's settings. To do this:
* in the repo for which notifications are being set, go to `Settings > Add webhook`
* add https://services.w3.org/github-notify-ml/ where it says `Payload URL`
* set `Content-type` as application/json
* ignore the box `Secret`
* set radio to `Send me everything`
* leave `Active` checked
* and press `Add Webhook`

If you want to use a different text in the notifications, you can also provide pull requests that bring special per mailing list templates as described above.

