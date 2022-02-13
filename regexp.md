# Regular Expressions

<details open="open">
  <summary>Table of contents</summary>
  <ul>
    <li>
      <a href="#validations">Validations</a>
      <ul>
        <li>
          <a href="#number-ranges">Number ranges</a>
        </li>
        <li>
          <a href="#hex-color-code">Hex color code</a>
        </li>
      </ul>
    </li>
  </ul>
</details>

## Validations

### Number ranges

- example 1: `150-193` = `(150-189, 190-193)`

  ```
  1([5-8][0-9]|9[0-3])
  ```

- example 2: `256-512` = `(256-259, 260-299, 300-499, 500-509,510-512)`

  ```
  (25[6-9]|2[6-9][0-9]|[3-4][0-9][0-9]|50[0-9]|51[0-2])
  ```

### Hex color code

- Hex code = `#000-#fff, #000000-#ffffff`
  ```
  #([a-fA-F0-9]{6}|[a-fA-F0-9]{3})
  ```
