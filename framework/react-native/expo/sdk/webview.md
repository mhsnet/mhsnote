# [《MHS 笔记》] > [WebView]
> 本地视图渲染web[android|emulator|ios|simulator]

## 安装
```
$ expo install react-native-webview
```

## 使用
> 基本HTML内联
```
import { WebView } from 'react-native-webview';
...
return (
    <WebView
      originWhitelist={['*']}
      source={{ html: '<h1>你好</h1>' }}
      style={{ marginTop: 20 }}
    />
);
```
> 基本url源
```
import { WebView } from 'react-native-webview';
...
return (
    <WebView
      source={{ uri: 'https://www.baidu.com/' }}
      style={{ marginTop: 20 }}
    />
);
```
> JS和Native通信
```
# injectedJavaScript --- rn->web 页面第一次加载时运行
# injectJavaScript --- rn->web 

```
## 
[《MHS 笔记》] : https://mhsnet.github.io/mhsnote/ "《MHS 笔记》"

[WebView]: https://mhsnet.github.io/mhsnote/framework/react-native/expo/sdk/webview.html "WebView"