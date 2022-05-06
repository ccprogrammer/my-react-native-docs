# my-react-native-docs
  From flutter to React Native, i will put which code is from react or flutter by (in react) it's from left side and (in flutter) it's from right side

 ## # Props  / Constructor 
Props is short for “properties”. Props let you customize React components by passing parameter

<details>
 <summary> View Code </summary>


 
```
import React from 'react';
import { Text, View, Image } from 'react-native';
  
  const Cat = (props) => {
  return (
    <View>
      <Text>Hello, I am {props.name}!</Text>
    </View>
  );
}

const Cafe = () => {
  return (
    <View>
      <Cat name="Maru" />
      <Cat name="Jellylorum" />
      <Cat name="Spot" />
    </View>
  );
}

```
</details>
 
 
  ## # useState / setState
  
  For more explanation, there are 2 const variables that that have bool value true, in here {isHungry ? "hungry" : "full"} it means if isHungry still remains true it it will return text "hungry" if the state changed it will return "full", setIsHunry in button function is to change the isHungry state and for disabled in button it has the reverse value from isHungry from false at start when isHungry change then the button will change to true

<details>
 <summary> View Code </summary>

```
import React, { useState } from "react";
import { Button, Text, View } from "react-native";

  
const Cat = (props) => {
  const [isHungry, setIsHungry] = useState(true);

  return (
    <View>
      <Text>
        I am {props.name}, and I am {isHungry ? "hungry" : "full"}!
      </Text>
      <Button
        onPress={() => {
          setIsHungry(false);
        }}
        disabled={!isHungry}
        title={isHungry ? "Pour me some milk, please!" : "Thank you!"}
      />
    </View>
  );
}

const Cafe = () => {
  return (
    <>
      <Cat name="Munkustrap" />
      <Cat name="Spot" />
    </>
  );
}
      
```
 
</details>

 
## # Template

<details>
 <summary> View Code </summary>

 
```

```
 
</details>
 
 ---
 
 
 
 
  ## # Template

<details>
 <summary> View Code </summary>

 
```

```
 
</details>

