# Getting Started with Scrapbook - a dynamic coding environment.

## What is Scrapbook, and what does it do?

- It's a full-featured in-browser IDE and markdown editor for documentation.
- You can import any npm module in the IDE. The bundling and transpiling of your code are handled in the browser.
- React and ReactDOM are already imported and ready for use.
  ![sample](https://github.com/dannysarco/code-editor/assets/54184032/ff98a6a8-d055-40a1-a2c7-836bb4f24e8a)

## To Use Scrapbook

- Click the **+ Code** or **+Text** button at the top of the screen to get started!
  ![blank](https://github.com/dannysarco/code-editor/assets/54184032/5f32d564-f338-42d8-bacc-4b5a881dcc0e)
  ![emptycells](https://github.com/dannysarco/code-editor/assets/54184032/f1aafc94-92c7-4bd2-b6df-07c76eb3b889)

## Markdown sample text for the text editor that contains an "Explainer".

```
**Scrapbook**
----------
This is an interactive coding environment. You can write Javascript, see it executed, and write comprehensive documentation using markdown.

- Click any text cell (including this one) to edit it
- The code in each code editor is joined into one file. If you define a variable in cell #1, you can refer to it in any of the following cells!
- Click the **Format** button in any code cell, and Prettier will its thing to your code!
- You can show any React component, string, number, or anything else by calling the `show` function. This is a function built into this environment. Call show multiple times to show multiple values
- Re-order or delete cells using the buttons on the top right
- Add new cells by hovering on the divider between each cell

```

## Code samples for the code editor.

```
import { useState } from 'react';

const Counter = () => {
  const [count, setCount] = useState(0);
  return (
    <div>
      <button onClick={() => setCount(count + 1)}>Click</button>
      <h3>Count: {count}</h3>
    </div>
  );
};
// Display any variable or React Component by calling 'show'
show(<Counter />);

```

```
  import axios from 'axios';
  import 'bulma/css/bulma.css';

  axios.get('http://jsonplaceholder.typicode.com/users/1')
  .then(({ data }) => show(data.name));
```

## Future Functionality

- Lots! This is just the beginning.
