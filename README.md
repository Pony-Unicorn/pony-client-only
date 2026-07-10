# tiny-client-only

A lightweight React component that renders its children **only on the client side**, helping avoid SSR hydration errors in frameworks like Next.js.

Copied from https://diceui.com/docs/utilities/base/client-only

## 📦 Installation

```bash
npm install tiny-client-only
# or
pnpm add tiny-client-only
```

## 🚀 Usage

```tsx
import ClientOnly from "tiny-client-only";

export default function Page() {
  return (
    <ClientOnly>
      <div>This will only render on the client!</div>
    </ClientOnly>
  );
}
```

You can also provide a custom fallback while waiting for the client to load:

```tsx
<ClientOnly fallback={<span>Loading...</span>}>
  <ExpensiveChart />
</ClientOnly>
```

## ⚙️ Build (for maintainers)

```bash
pnpm install
pnpm run build
```

## 🪪 License

MIT © Pony
