# Week challenges (Monday) 💻
Time to catch up ⏱️
# Week challenges (Tuesday) 💻
Time to catch up ⏱️
# Week challenges (Wednesday) 💻
1. [x] Watch this What Is React (React js) & Why Is It So Popular? video
Notes: 
* A piece of User Interface (UI) - library created from Facebook since 2011
* We no longer have to write "addEventListener" and instead manipulate the DOM and updates it.
* Angular is more a framework solution.
* Whereas React only takes care of the view of the library. Views and syncs with sate for routing, HTTPS services and API to learn.
3. [x] Watch this Learn React video

To review which version of NODE i have installed in my terminal:
``` 
node -v 
```

To create a new react app:
``` 
npx create-react-app 
```

To start creating
``` 
npm start
```

UUID Package install:
```
install UUID
```

# Week challenges (Thursday) 💻
3. [ ] React kata
```Typescript
import React from 'react';

export const EggList = (props) => {
  //1. Set a list with properties called eggs in an array[]
  const eggs = ["Lindt", "BlackChoco", "WhiteChoco"]
  //2. Loop through the prop.eggs to output an unorder list of the Easter eggs
  const propEggs = props.eggs;
  return propEggs.reverse()
  
};

export const EasterEgg = (props) => {
  //3. List item with property name, to render the name<li></html> tag
  const listedEastEgg = props.EasterEgg
  //4. Each EasterEgg needs a key prop with an unique getElementById
  return (<li key={listedEastEgg}>props.listedEastEgg</li>)
};
```
