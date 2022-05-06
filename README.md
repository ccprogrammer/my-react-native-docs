# my-react-native-docs
  From flutter to React Native, i will put which code is from react or flutter by (in react) it's from left side and (in flutter) it's from right side

 ## # Props  / Constructor 
Props is short for “properties”. Props let you customize React components by passing parameter

<details>
 <summary> View Code </summary>


 
```
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
  
  For more explanation, there are 2 const variables that that have bool value true, in here {isHungry ? "hungry" : "full"} it means if isHungry still remains true it it will return text "hungry" if the state changed it will return "full", the function to change the state in in the button  setIsHungry(false); and for disabled it's mean the button will go into disabled state if isHungry = false

<details>
 <summary> View Code </summary>

```
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

 
 
 ---
 
 
 
 
  ## # Template

<details>
 <summary> View Code </summary>

 
```

```
 
</details>

