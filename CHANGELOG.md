# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added
- JSON Web Token support.
``` json 
    // .livego.json
    {
        "jwt": {
            "secret": "testing",
            "algorithm": "HS256s"
        },
        "server": [
            {
                "appname": "live",
                "liveon": "on",
                "hlson": "on"
            }
        ]
    }
```
- Use redis for store room keys
``` json 
    // .livego.json
    {
        "redis_addr": "localhost:6379", 
        "server": [
            {
                "appname": "live",
                "liveon": "on",
                "hlson": "on"
            }
        ]
    }
```

### Changed
- Show `players`.
- Show `stream_id`.