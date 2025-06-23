![Logo](/GoFakeS3.png)

[![Build Status](https://github.com/oneclickvirt/gofakes3/workflows/build/badge.svg)](https://github.com/oneclickvirt/gofakes3/actions?query=workflow%3Abuild)
[![Go Report Card](https://goreportcard.com/badge/github.com/oneclickvirt/gofakes3)](https://goreportcard.com/report/github.com/oneclickvirt/gofakes3)
[![GoDoc](https://pkg.go.dev/badge/github.com/oneclickvirt/gofakes3.svg)](https://pkg.go.dev/github.com/oneclickvirt/gofakes3)

This is a fork of [johannesboyne/gofakes3](https://github.com/johannesboyne/gofakes3)
mainly for use implementing the [rclone serves3](https://rclone.org/commands/rclone_serve_s3/) command in
[rclone/rclone](https://github.com/rclone/rclone).

Notable differences:

* Use modified xml library to handle more control chars
* Func `getVersioningConfiguration` will return empty when unversioned
* New func in `backend` interface: `CopyObject`
* Support authentication with AWS Signature V4 
* Interfaces changed to take context
