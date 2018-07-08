# react-cristal
> Convert any component into a window

<div align="center">
  <img src="demo.gif" alt="demo">
  <br><br>
</div>

# Demo 🍿

[https://zzarcon.github.io/react-cristal](https://zzarcon.github.io/react-cristal)

# Features ✨

* Draggable
* Resizable
* Automatically stacking
* Smart positions
* Window boundaries restriction

# Install 🚀

```
$ yarn add react-cristal
```

# Usage ⛏

**Basic** 

```tsx
import Cristal from 'react-cristal';

<Cristal>
  Look at me, I'm inside a window!
</Cristal>
```

**Custom**

```tsx
import Cristal from 'react-cristal';

<Cristal
  title="Some title"
  initialPosition="top-center"
  isResizable={false}
  onClose={() => console.log('close clicked')}
>
  <div>
    Some content
  </div>
</Cristal>
```

# Api 📚

```ts
export type InitialPosition = 'top-left' | 'top-center' | 'top-right' | 'bottom-left' | 'bottom-center' | 'bottom-right' | 'center';

interface Props {
  children: ReactNode;
  title?: string;
  initialPosition?: InitialPosition;
  isResizable?: boolean;
  onClose?: () => void;
  className?: string;
}
```

See [example/](https://github.com/zzarcon/react-cristal/tree/master/example) for full example.

# Author

[@zzarcon](https://twitter.com/zzarcon)