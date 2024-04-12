
![Logo](/GoFakeS3.png)

This is a fork of [johannesboyne/gofakes3](https://github.com/johannesboyne/gofakes3)
mainly for use implementing the [rclone serves3](https://rclone.org/commands/rclone_serve_s3/) command in
[rclone/rclone](https://github.com/rclone/rclone).

Notable differences:

* Use modified xml library to handle more control chars
* Func `getVersioningConfiguration` will return empty when unversioned
* New func in `backend` interface: `CopyObject`
* Support authentication with AWS Signature V4 
* Interfaces changed to take context
