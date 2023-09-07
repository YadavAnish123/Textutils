# Textutils
 'React' web application named "Textutils":

---


## Overview

Textutils is a React web application that facilitates the manipulation of text. It offers features such as changing the case of a sentence, 
eliminating unused spaces, and clearing the text content.

## Features

- **Change Case**: Convert text to various cases like uppercase, lowercase, sentence case, etc.
- **Eliminate Unused Space**: Remove extra spaces and ensure clean and consistent formatting.
- **Clear Text**: Quickly clear the content in the text area.
- #enable darkmode

## Getting Started

1. Clone the repository:

```bash
git clone https://github.com/yourusername/textutils.git
```

2. Navigate to the project directory:

```bash
cd textutils
```

3. Install dependencies:

```bash
npm install
```

4. Start the application:

```bash
npm start
```

5. Open your web browser and go to `http://localhost:3000` to use Textutils.

## Usage

1. Enter or paste the text you want to manipulate in the provided text area.
2. Use the buttons to apply different transformations (Change Case, Eliminate Unused Space, Clear Text).

## Example

```jsx
import React, { useState } from 'react';
import { CaseConverter, SpaceEliminator } from './Textutils';

function App() {
  const [inputText, setInputText] = useState('');

  const handleInputChange = (e) => {
    setInputText(e.target.value);
  };

  return (
    <div>
      <textarea value={inputText} onChange={handleInputChange} />
      <CaseConverter text={inputText} />
      <SpaceEliminator text={inputText} />
    </div>
  );
}

export default App;
```

## Dependencies

- React
- Additional dependencies are listed in `package.json`.

## Contributing

If you'd like to contribute to this project, please fork the repository and submit a pull request. Issues and feature requests are also welcome!

 
