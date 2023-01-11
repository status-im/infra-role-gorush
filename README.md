# Description

This role configures a [gorush](https://github.com/appleboy/gorush) which can talk to Goolg and Apple backends for delivering mobile notifications.

# Configuration

Currently the configuration supports only iOS notifications and it requires:
```yaml
# iOS API access key in one of 3 formats: pem, p12 or p8
gorush_ios_key_contents: '<contents of the p8 key file>'
# KeyID from developer account (Certificates, Identifiers & Profiles -> Keys)
gorush_ios_key_id: '<ios_key_id>'
# TeamID from developer account (View Account -> Membership)
gorush_ios_team_id: '<ios_team_id>'
```

# Known Issues

* Despite Android support being disabled the `android.apikey` has to have any value
