# Snippety

This extension provides you with Snippets for all web programming frameworks such as React, Redux, Vue, Angular, Flask, Django and much more[VS Code](https://code.visualstudio.com/)

## Languages

Snippety provides support for the following languages:

- JavaScript
  - React
  - ES7
  - TypeScript
  - Vue
  - Angular
  - Next
  - Lodash
  - GraphQL
  - Express
- Python
  - Flask
  - Django

### Visual Studio Marketplace

Launch *Quick Open*:

- [_Linux_](https://code.visualstudio.com/shortcuts/keyboard-shortcuts-linux.pdf): `Ctrl+P`
- [_macOS_](https://code.visualstudio.com/shortcuts/keyboard-shortcuts-macos.pdf): `⌘P`
- [_Windows_](https://code.visualstudio.com/shortcuts/keyboard-shortcuts-windows.pdf): `Ctrl+P`

Paste the following command and press `Enter`:

```
ext install japrozsaini.snippety

```

### GitHub Repository Clone

Change to your `.vscode/extensions` [VS Code extensions directory](https://code.visualstudio.com/docs/extensions/install-extension#_side-loading). Depending on your platform it is located in the following folders:

- _Linux_: `~/.vscode/extensions`
- _macOS_: `~/.vscode/extensions`
- _Windows_: `%USERPROFILE%\.vscode\extensions`

Clone the Material Theme repository as `dsznajder.es7-react-js-snippets`:

```
git clone https://github.com/Japroz-Saini/Snippety

```

Here is direct link to marketplace [ES7 React/Redux/React-Native/JS Snippets](https://marketplace.visualstudio.com/items?itemName=JaprozSinghSaini.snippety)

## Supported languages (file extensions)

- JavaScript (.js)
- JavaScript React (.jsx)
- TypeScript (.ts)
- TypeScript React (.tsx)
- Vue (.vue)
- Angular (.ts)
- HTML (.html)
- Python (.py)

## Commands

Various Commands with their snippets

#### rfce

Generates a ReactJS functional Component

```javascript
import React from "react";

function nav() {
  return <div></div>;
}

export default nav;
```

### Vaction

Generates a Standard VueX Action

```javascript
actions: {
    updateValue({commit}, payload) {
        commit('updateValue', payload);
    }
}

```

### a-guard-can-activate

Generates an angular Snippets

```javascript
import { Injectable } from "@angular/core";
import {
  ActivatedRouteSnapshot,
  CanActivate,
  RouterStateSnapshot,
} from "@angular/router";

@Injectable({ providedIn: "root" })
export class NameGuard implements CanActivate {
  constructor() {}

  canActivate(route: ActivatedRouteSnapshot, state: RouterStateSnapshot) {
    return true;
  }
}
```

### next-api-method

Generates a snippet for a next-api method

```javascript
export default (req, res) => {
  if (req.method === "POST") {
  } else {
  }
};
```

### Redux

Generates Redux Snippets for ReactJS

```javascript
const mapStateToProps = (state) => ({});

const mapDispatchToProps = {};
```

### Python

Can generate Python Code such as below:

```python

class Robot:
    '''Represents a robot, with a name.'''
    # A class variable, counting the number of robots
    population = 0
    def __init__(self, name):
        '''Initializes the data.'''
        self.name = name
        print('(Initializing {})'.format(self.name))
        # When this person is created, the robot
        # adds to the population
        Robot.population += 1
    def die(self):
        '''I am dying.'''
        print('{} is being destroyed!'.format(self.name))
        Robot.population -= 1
        if Robot.population == 0:
            print('{} was the last one.'.format(self.name))
        else:
            print('There are still {:d} robots working.'.format(
                Robot.population))
    def say_hi(self):
        '''Greeting by the robot.
        Yeah, they can do that.'''
        print('Greetings, my masters call me {}.'.format(self.name))
    @classmethod
    def how_many(cls):
        '''Prints the current population.'''
        print('We have {:d} robots.'.format(cls.population))
droid1 = Robot('R2-D2')
droid1.say_hi()
Robot.how_many()
droid2 = Robot('C-3PO')
droid2.say_hi()
Robot.how_many()
print('Robots can do some work here.')
print('Robots have finished their work. So lets destroy them.')
droid1.die()
droid2.die()
Robot.how_many()
```
