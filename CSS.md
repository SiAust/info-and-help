# CSS

### SCSS

Allows extra formatting and easy syntax. Be sure to use "Live SASS/SCSS compiler" extension.

<hr>

### `&` operator (SASS/SCSS feature)

```scss
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

is equivalent to

```css
.opinions_box {
  margin: 0 0 8px 0;
  text-align: center;
}

.opinions_box__view-more {
  text-decoration: underline;
}

.opinions_box__text_input {
  border: 1px solid #ccc;
}

.opinions_box--is-active {
  color: gray;
}
```

<hr>
