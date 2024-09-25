# Table of Contents

1. [Cursor + Selecting](#cursor)
2. [Deleting](#deleting)
3. [Find & Replace](#find--replace)
4. [Formatting](#formatting)
5. [Macros](#macros)
6. [Other](#other)
7. [Panes](#panes)
8. [Searching](#searching)
9. [Tabs](#tabs)

---

## Cursor + Selecting

- **Go to the start of the line:**  
  `"0"`

- **Go to the end of the line:**  
  ```$```

- **Go to the middle of the line:**  
  ```gM```

- **Jump between (), [], {}, etc**  
  `%`

- **Go to the start of file:**  
  `gg`

- **Go to the end of file:**  
  `G`

- **Move cursor to character (forward):**  
  `f<character>`

- **Move cursor to character (backward):**  
  `F<character>`

- **Paste from keyboard:**  
  `<leader> + p`

- **Select content inside (), [], {}, etc**  
  `v` + `i` + `open delimiter`

- **Replace content inside (), [], {}, etc, with yanked line**  
  `v` + `i` + `open delimiter` + `p`

---

## Deleting

- **Delete forwards until a character:**  
  `d + f + <character>`

- **Delete backwards until a character:**  
  `d + F + <character>`

---

## Find & Replace

1. Place cursor over the word.
2. Press `*`.
3. Type `ciw` (change inner word).
4. Type the new word (replacing the word).
5. Press `n` (move to next occurrence).
6. Press `.` (repeat the last step).

- **Replace current cursor word with yanked line**  
  `viw` + `p`

---

## Formatting

- **Indent a file:**  
  `gg + '=' + G`

- **Sort highlighted lines:**  
  `:sort`

- **Join two lines:**  
  `J`

---

## Macros

- **Record a macro:**  
  `qq + <some macro> + esc + q`

- **Play a macro:**  
  `@q`

- **Replay last used macro:**  
  `@@`

---

## Other

- **Open url link in browser:**  
  `gx`

- **Join two lines**  
  `J`

#### Vim marks
- **Place mark - current file**  
  `m` + `<lowercase register>`

- **Place mark - global file**  
  `m` + `<uppercase register>`

- **Goto mark**  
  `'` + `<register>`

---

## Panes

- **Create vertical pane:**  
  `<leader> + %`

- **Create horizontal pane:**  
  `<leader> + " `

- **Maximize current window width:**  
  `<C-w> + "|"`

- **Maximize current window height:**  
  `<C-w> + "_"`

- **Increase current window width:**  
  `<C-w> + ">"`

- **Decrease current window width:**  
  `<C-w> + "<"`

- **Increase current window width (by number):**  
  `"number" + <C-w> + ">"`

---

## Searching

- **Find occurrence of word:**  
  `"/" + <word> + enter`

- **Next occurrence:**  
  `n`

- **Previous occurrence:**  
  `N`

- **Go to function definition:**  
  `<leader> + ]`

---

## Tabs

- **Create new tab:**  
  `<C-w> + t`

- **Next tab:**  
  `<C-w> + n`

- **Previous tab:**  
  `<C-w> + p`

