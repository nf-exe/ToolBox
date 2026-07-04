# tr

## What is `tr`?

`tr` (translate) is a Linux command used to **translate, replace, delete, or squeeze characters** from standard input.

Unlike many commands, `tr` **does not read files directly**, so it's commonly used with pipes (`|`).

---

## Common Uses

- Replace characters
- Convert lowercase to uppercase
- Convert uppercase to lowercase
- Delete characters
- Remove duplicate consecutive characters

---

## Examples

### Convert lowercase to uppercase

```bash
echo "hello world" | tr 'a-z' 'A-Z'
```

Output:

```text
HELLO WORLD
```

---

### Convert uppercase to lowercase

```bash
echo "HELLO" | tr 'A-Z' 'a-z'
```

Output:

```text
hello
```

---

### Delete digits

```bash
echo "abc123" | tr -d '0-9'
```

Output:

```text
abc
```

---

### Remove repeated spaces

```bash
echo "Hello     World" | tr -s ' '
```

Output:

```text
Hello World
```

