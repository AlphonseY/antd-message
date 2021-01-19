# message-like-antd

A message component like `Antd`. If you want use a message component, but not want import the whole `Antd`, you can try it.

## Install

```javascript
  npm install message-like-antd
  yarn add message-like-antd
```

## Import

Use in NPM:

```javascript
  import $message from 'message-like-antd'
  import 'message-like-antd/src/theme/message.css'
```

Use in HTML:

```html
  <link ref="stylesheet" href="./message-like-antd/dist/theme/message.css" />
  <script src="./message-like-antd/dist/message.js"></script>
```

## API

```javascript
  $message.success(content, [duration], onClose)
  $message.error(content, [duration], onClose)
  $message.info(content, [duration], onClose)
  $message.warning(content, [duration], onClose)
  $message.loading(content, [duration], onClose)
  $message.destroy() // destroy all message

  let message = $message.success(content, [duration], onClose)
  message() // destroy single
```

Argument descripton

Argument|Description|Type|Default
:--|:--|:--|:--
content|content of the message|string|-
duration|time(seconds) before auto-dismiss, don't dismiss if set to 0|number|3
onClose|Specify a function that will be called when the message is closed|Function|-
