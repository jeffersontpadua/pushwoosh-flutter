## Installation

1) Install the library from pub:

```yaml
dependencies:
  pushwoosh: '^1.8.0'
```

2) Configure Firebase Android project in [Firebase console](https://console.firebase.google.com).

3) Place a google-services.json file into android/app folder in your project directory.

## Usage

```dart
import 'package:pushwoosh/pushwoosh.dart';
...
Pushwoosh.initialize({"app_id": "YOUR_APP_ID", "sender_id": "FCM_SENDER_ID"});
Pushwoosh.getInstance.onPushReceived.listen((event) {
...
});
Pushwoosh.getInstance.onPushAccepted.listen((event) {
...
});
Pushwoosh.getInstance.registerForPushNotifications();
```