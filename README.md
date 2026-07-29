<p align="center">
  <a href="https://github.com/lucide-icons/lucide#gh-light-mode-only">
    <img src="assets/image.png" alt="Lucide - Beautiful & consistent icon toolkit made by the community. Open-source project and a fork of Feather Icons." width="480">
  </a>
</p>

<p align="center">
  <a href="https://github.com/bilalbentoumi/expo-ui-lucide-icons/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-ISC-green" alt="license"></a>
  <a href="https://www.npmjs.com/package/expo-ui-lucide-icons"><img src="https://img.shields.io/npm/v/expo-ui-lucide-icons" alt="npm version"></a>
  <img src="https://img.shields.io/npm/dw/expo-ui-lucide-icons" alt="npm downloads">
</p>

<p align="center">
  <a href="https://lucide.dev/icons/">Icons</a>
  ·
  <a href="https://lucide.dev/guide/">Guide</a>
  ·
  <a href="https://lucide.dev/packages">Packages</a>
  ·
  <a href="https://lucide.dev/license">License</a>
</p>

# expo-ui-lucide-icons

**Lucide icons as Android Vector Drawables for Expo / React Native**

A collection of 1600+ [Lucide](https://lucide.dev) icons exported as Android Vector Drawable (XML) files, ready to use in Expo and React Native projects.

This package ships raw `.xml` vector drawables bundled as TypeScript/JavaScript modules, allowing you to import individual icons and render them with libraries like [`react-native-svg`](https://github.com/software-mansion/react-native-svg) or any drawable-compatible renderer.

## Installation

```bash
npm install expo-ui-lucide-icons
# or
yarn add expo-ui-lucide-icons
```

## Usage

Each icon is a named export pointing to an Android Vector Drawable XML string.

```ts
import { CameraIcon, HeartIcon, StarIcon } from "expo-ui-lucide-icons";

console.log(CameraIcon); // XML string of the camera vector drawable
```

### With `@expo/ui` Icon

Use the `Icon` component from `@expo/ui` to render icons natively:

```tsx
import { Host, Icon } from "@expo/ui";
import { CameraIcon } from "expo-ui-lucide-icons";

export default function App() {
  return (
    <Host matchContents>
      <Icon source={CameraIcon} size={32} color="orange" />
    </Host>
  );
}
```

## Available Icons

The package includes all **1600+ Lucide icons**. Browse them at [lucide.dev/icons](https://lucide.dev/icons/).

All icons follow the naming convention: `{IconName}Icon`. For example:

- `camera` → `CameraIcon`
- `heart` → `HeartIcon`
- `arrow-down-circle` → `ArrowDownCircleIcon`

## License

Lucide is licensed under the [ISC License](https://github.com/lucide-icons/lucide/blob/main/LICENSE). Free for commercial and personal use.

## Credits

- Icons by [Lucide](https://lucide.dev)
- All Lucide contributors on [GitHub](https://github.com/lucide-icons/lucide/graphs/contributors)
