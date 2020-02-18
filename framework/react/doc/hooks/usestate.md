# [《MHS 笔记》] > [useState]

## useState
```
# 返回状态和更新状态函数 
# state --- 状态（更新[obj,arr] - 替换非合并）
# setState --- 更新状态函数
# initialState --- state初始值
const [state, setState] = useState(initialState);
```

## 使用setState
> 1. 例
```
# App.tsx
import React, { useState } from 'react';
import { Button, StyleSheet, Text, View } from 'react-native';

export default function App() {
  const [count, setCount] = useState(0);
  // const [count, setCount] = useState(()=>{
  //   return 0;
  // });
  return (
    <View style={styles.container}>
      <Text>点击{count}次</Text>
      <Button title="点击" onPress={() => setCount(count + 1)} />
    </View>
  );
}

const styles = StyleSheet.create({
  container: {
    flex: 1,
    backgroundColor: '#fff',
    alignItems: 'center',
    justifyContent: 'center',
  },
});
```
> 2. 函数组件中使用，可替类
```
# 使用1
const Example = (props) => {}
# 使用2
function Example(props) {}
```


## 
[《MHS 笔记》]: https://mhsnet.github.io/mhsnote/ "《MHS 笔记》"

[useState]: https://mhsnet.github.io/mhsnote/framework/react/doc/hooks-usestate.html "useState"