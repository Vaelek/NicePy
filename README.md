# NicePy

A python package for the CXOnce NICE/inContact API

This is a work in progress and currently far from complete in terms of endpoints. More will be added over time.

# Installation
`pip install nicepy`

Functions that involve media may require one or both of `ffprobe` and `ffmpeg` to be in the system path. If you receive a file not found error this is likely the reason.

## Configuration
* In your project folder, create a file `nicepy_config.json` containing the following:

```json
{
  "client_id" : "APP_ID",
  "client_secret" : "APP_SECRET",
  "username" : "USER_ID",
  "password" : "USER_SECRET",
  "APIVersion" : "28.0"
}
```

`client_id` and `client_secret` are the keys provided when registering an API app with NICE. `username` and `password` are the keys generated on a user account within NICE.

`APIVersion` if not set will default to v28.0. All endpoints with versioning (will) allow passing a version in the call.

