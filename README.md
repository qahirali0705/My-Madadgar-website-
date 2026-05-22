# My-Madadgar-website-
@import "tailwindcss" source(none);
@source "../src";
@import "tw-animate-css";

@custom-variant dark (&:is(.dark *));

@theme inline {
  --radius-sm: calc(var(--radius) - 4px);
  --radius-md: calc(var(--radius) - 2px);
  --radius-lg: var(--radius);
  --radius-xl: calc(var(--radius) + 4px);
  --radius-2xl: calc(var(--radius) + 8px);
  --color-background: var(--background);
  --color-foreground: var(--foreground);
  --color-card: var(--card);
  --color-card-foreground: var(--card-foreground);
  --color-popover: var(--popover);
  --color-popover-foreground: var(--popover-foreground);
  --color-primary: var(--primary);
  --color-primary-foreground: var(--primary-foreground);
  --color-primary-glow: var(--primary-glow);
  --color-secondary: var(--secondary);
  --color-secondary-foreground: var(--secondary-foreground);
  --color-accent: var(--accent);
  --color-accent-foreground: var(--accent-foreground);
  --color-muted: var(--muted);
  --color-muted-foreground: var(--muted-foreground);
  --color-destructive: var(--destructive);
  --color-destructive-foreground: var(--destructive-foreground);
  --color-border: var(--border);
  --color-input: var(--input);
  --color-ring: var(--ring);
  --color-surface: var(--surface);
  --color-surface-elevated: var(--surface-elevated);
  --font-sans: "Inter", "ui-sans-serif", system-ui, sans-serif;
  --font-display: "Plus Jakarta Sans", "Inter", system-ui, sans-serif;
}

:root {
  --radius: 0.875rem;
  --background: oklch(0.985 0.012 85);
  --foreground: oklch(0.22 0.025 160);
  --surface: oklch(1 0 0);
  --surface-elevated: oklch(0.99 0.008 90);
  --card: oklch(1 0 0);
  --card-foreground: oklch(0.22 0.025 160);
  --popover: oklch(1 0 0);
  --popover-foreground: oklch(0.22 0.025 160);
  --primary: oklch(0.52 0.14 158);
  --primary-foreground: oklch(0.985 0.012 85);
  --primary-glow: oklch(0.68 0.16 158);
  --secondary: oklch(0.94 0.02 90);
  --secondary-foreground: oklch(0.28 0.03 160);
  --accent: oklch(0.78 0.16 70);
  --accent-foreground: oklch(0.22 0.04 60);
  --muted: oklch(0.95 0.01 90);
  --muted-foreground: oklch(0.5 0.02 160);
  --destructive: oklch(0.58 0.22 25);
  --destructive-foreground: oklch(0.985 0.012 85);
  --border: oklch(0.9 0.012 90);
  --input: oklch(0.92 0.012 90);
  --ring: oklch(0.52 0.14 158);
  --gradient-hero: linear-gradient(135deg, oklch(0.52 0.14 158) 0%, oklch(0.68 0.16 158) 50%, oklch(0.78 0.16 70) 100%);
  --gradient-card: linear-gradient(180deg, oklch(1 0 0) 0%, oklch(0.985 0.012 85) 100%);
  --shadow-soft: 0 1px 2px oklch(0.22 0.025 160 / 0.06), 0 4px 16px oklch(0.22 0.025 160 / 0.06);
  --shadow-glow: 0 8px 40px oklch(0.52 0.14 158 / 0.25);
}

.dark { /* dark mode tokens */ }

@layer base {
  * { border-color: var(--color-border); }
  html, body { font-family: var(--font-sans); }
  body { background-color: var(--color-background); color: var(--color-foreground); -webkit-font-smoothing: antialiased; }
  h1, h2, h3, h4 { font-family: var(--font-display); letter-spacing: -0.02em; }
}

@layer utilities {
  .bg-hero { background: var(--gradient-hero); }
  .bg-card-gradient { background: var(--gradient-card); }
  .shadow-soft { box-shadow: var(--shadow-soft); }
  .shadow-glow { box-shadow: var(--shadow-glow); }
  .text-balance { text-wrap: balance; }
}
