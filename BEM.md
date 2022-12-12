# Blocks, Elements and Modifiers

## Block

Standalone entity that is meaningful on its own.

Examples
header, container, menu, checkbox, input

## Element

A part of a block that has no standalone meaning and is semantically tied to its block.

Examples
menu item, list item, checkbox caption, header title

## Modifier

A flag on a block or element. Use them to change appearance or behavior.

Examples
disabled, highlighted, checked, fixed, size big, color yellow

- Before

```css
#opinions_box h1 {
  margin: 0 0 8px 0;
  text-align: center;
}

#opinions_box {
  p.more_pp {
    a {
      text-decoration: underline;
    }
  }

  input[type="text"] {
    border: 1px solid #ccc !important;
  }
}
```

- After

```css
.opinions_box {
  margin: 0 0 8px 0;
  text-align: center;

  &__view-more {
    text-decoration: underline;
  }

  &__text-input {
    border: 1px solid #ccc;
  }

  &--is-inactive {
    color: gray;
  }
}
```

TODO: Add citation
