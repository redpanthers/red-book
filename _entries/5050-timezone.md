---
sectionid: timezone
sectionclass: h2
title: Timezone Management
parent-id: ror
number: 5050
---

**DON’T USE**

```
  * Time.now
  * Date.today
  * Date.today.to_time
  * Time.parse("2015-07-04 17:05:37")
  * Time.strptime(string, "%Y-%m-%dT%H:%M:%S%z")
```

**USE**

```
* Time.current
* 2.hours.ago
* Time.zone.today
* Date.current
* 1.day.from_now
* Time.zone.parse("2015-07-04 17:05:37")
* Time.strptime(string, "%Y-%m-%dT%H:%M:%S%z").in_time_zone
```

You can read more about it from our [blog](http://blog.redpanthers.co/working-timezones-rails/)