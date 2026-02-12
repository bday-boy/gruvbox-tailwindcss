# Gruvbox for [TailwindCSS](https://github.com/tailwindlabs/tailwindcss)

A [Gruvbox](https://github.com/morhetz/gruvbox) color palette for use with
Tailwind CSS.

Big thank you to the creators and maintainers of the
[Catppuccin for TailwindCSS](https://github.com/catppuccin/tailwindcss)
repository, which I blatantly ripped the SASS code from to make this theme. I
don't actually know SASS at all, so they saved me the time it would've taken
to learn it from scratch.

## Usage

1. Download the gruvbox.css file
2. Import the theme in the same file as your `tailwindcss` import
3. Use it in your html

```css
@import "tailwindcss";
@import "./gruvbox.css";
```

```html
<!-- All colours are prefixed with `grv` -->
<body class="bg-grv-base">
  <h1 class="text-grv-text">Welcome!</h1>

  <!-- Gradients are supported too -->
  <button
    class="bg-linear-60 from-grv-green to-grv-aqua text-grv-base hover:from-grv-green-bright hover:to-grv-aqua-bright"
  >
    Click Here
  </button>

  <!-- 
  Flavour variants are predefined (`latte`, `frappe`, `macchiato`, and `mocha`)
  which allows you to force specific flavours and support custom theme switchers.
  -->
  <div class="dark">
    <p class="bg-grv-base text-grv-text">Hello from dark mode!</p>
  </div>
</body>
```
