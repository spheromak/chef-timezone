# Description

Provides LWRP to manage timezone.

# Requirements

## Platform

Only tested on Debian 6.

## Chef version

Chef version >= `0.10.10` has to be used.

# Usage

This cookbook has been designed to provide **LWRP** for your own infrastructure recipes.
Load this cookbook by your chef-client either by adding the line `depends "timezone"` to your infrastructure cookbook's metadata.rb file or by addind `recipe[timezone]` to your run\_list before the cookbook where you plan to use it. 

## LWRP

### timezone

This resource sets the timezone by editing `/etc/timezone` file and running `dpgk-reconfigure` afterwards.

```ruby
timezone "Europe/Moscow"
```

# License and Author

Author:: Kirill Kouznetsov (<agon.smith@gmail.com>)
Copyright:: 2013, Kirill Kouznetsov.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and

