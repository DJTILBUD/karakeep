# Module: tooling/tailwind

Provides shared Tailwind CSS configuration presets, offering a shared base configuration along with specialized presets for web and React Native/NativeWind applications.

## Key files
- `tooling/tailwind/base.ts`: Defines core Tailwind CSS configuration including dark mode strategy and shared content paths.
- `tooling/tailwind/native.ts`: Tailwind configuration preset extending base configuration with NativeWind theme extensions like hairline border widths.
- `tooling/tailwind/web.ts`: Tailwind configuration preset extending base configuration with web-specific animation keyframes, border radius CSS variables, typography, and animation plugins.

## Public interface
- default export in tooling/tailwind/base.ts: base Tailwind CSS configuration object
- default export in tooling/tailwind/native.ts: NativeWind-compatible Tailwind CSS configuration preset
- default export in tooling/tailwind/web.ts: Web-compatible Tailwind CSS configuration preset with typography and animate plugins

## Dependencies
- tailwindcss
- nativewind/theme
- @tailwindcss/typography
- tailwindcss-animate

## Open questions
- _none_
