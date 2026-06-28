# Caprine Notify for Home Assistant

Caprine Notify lets Home Assistant send rich local notifications to Caprine on Windows.

It provides the `caprine_notify.send_notification` action with support for:

- title and message
- persistent notifications
- custom timeout
- click URL
- custom icon
- optional silent mode
- automatic Caprine discovery over Zeroconf

Caprine must be running on the target PC with Home Assistant notifications enabled.

## Example

```yaml
action: caprine_notify.send_notification
data:
  title: Doorbell
  message: Someone is at the door.
  url: http://192.168.1.40:8123/local/tmp/doorbell_noification.jpg
  persistent: true
```
