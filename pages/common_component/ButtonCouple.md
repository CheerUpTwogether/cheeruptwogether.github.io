# ButtonCouple

### props
| option | **description** | **type** | **required** | **default** |
| --- | --- | --- | --- | --- |
| `textLeft` | 왼쪽 버튼 `text` | `string` | `true` |  |
| `textRight` | 오른쪽 버튼 `text` | `string` | `true` |  |
| `theme` | 왼쪽 버튼 색상 | `primary`<br/>`sub`<br/>`outline` | `false` | `primary` |
| `onPressLeft` | 왼쪽 버튼 클릭 시 동작하는 메소드 | `function` | `true` |  |
| `onPressRight` | 오른쪽 버튼 클릭 시 동작하는 메소드 | `function` | `true` |  |
| `disableLeft` | 왼쪽 버튼 disable 여부 | `boolean` | `false` | `false` |
| `disableRight` | 오른쪽 버튼 disable 여부 | `boolean` | `false` | `false` |
| `icon` | 버튼 아이콘 | `React.ReactNode` | `false` |  |
| `style` | 버튼 스타일 | `object` | `object[]` | `false` |  |

<br />

### exmple
```jsx
import React from 'react';
import {View} from 'react-native';
import {commonStyle} from '@/styles/common';
import ButtonCouple from '@/components/common/ButtonCouple';

const Home = () => {
  return (
    <View style={commonStyle.container}>
      <ButtonCouple
        onPressLeft={() => {}}
        textLeft="test"
        theme="outline"
        onPressRight={() => {}}
        textRight="test"
      />
      <ButtonCouple
        onPressLeft={() => {}}
        textLeft="test"
        theme="sub"
        onPressRight={() => {}}
        textRight="test"
        style={{marginVertical: 12}}
      />
      <ButtonCouple
        theme="sub"
        onPressLeft={() => {}}
        textLeft="test"
        disableLeft={true}
        onPressRight={() => {}}
        textRight="test"
        style={{marginVertical: 12}}
      />
      <ButtonCouple
        theme="sub"
        onPressLeft={() => {}}
        textLeft="test"
        onPressRight={() => {}}
        textRight="test"
        disableRight={true}
        style={{marginVertical: 12}}
      />
    </View>
  );
};

export default Home;

```
<figure><img width="493" alt="image" src="https://github.com/user-attachments/assets/23edb543-9e18-498e-ac81-129a200d1cdd"/></figure>
