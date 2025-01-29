# nanoid-dictionary
Predefined character sets to use with [nanoid](https://github.com/ai/nanoid). Used by [nanoid-generate](https://github.com/CyberAP/nanoid-generate).

[![npm](https://img.shields.io/npm/v/nanoid-dictionary)](https://www.npmjs.com/package/nanoid-dictionary)

A fork of [CyberAP/nanoid-dictionary](https://github.com/CyberAP/nanoid-dictionary).


## Install
Install nanoid and dictionary

`npm i @nichoth/nanoid @nichoth/nanoid-dictionary`

## Usage

Require a `customAlphabet` from `nanoid` and pass a string from the dictionary:

```js
import { customAlphabet } from '@nichoth/nanoid';
import { lowercase } from '@nichoth/nanoid-dictionary';

const lowercaseRandomString = customAlphabet(lowercase, 10);
```


## Character sets

### `numbers`

Numbers from 0 to 9

```javascript
import { numbers } from '@nichoth/nanoid-dictionary';
```

### `hexadecimalLowercase`

Lowercase English hexadecimal lowercase characters: `0123456789abcdef`

```javascript
import { hexadecimalLowercase } from '@nichoth/nanoid-dictionary';
```

### `hexadecimalUppercase`

Lowercase English hexadecimal uppercase characters: `0123456789ABCDEF`

```javascript
import { hexadecimalUppercase } from '@nichoth/nanoid-dictionary';
```

### `lowercase`

Lowercase English letters: `abcdefghijklmnopqrstuvwxyz`

```javascript
import { lowercase } from '@nichoth/nanoid-dictionary';
```

### `uppercase`

Uppercase English letters: `ABCDEFGHIJKLMNOPQRSTUVWXYZ`

```javascript
import { uppercase } from '@nichoth/nanoid-dictionary';
```

### `alphanumeric`

Combination of all the lowercase, uppercase characters and numbers from 0 to 9

Does not include any symbols or special characters

```javascript
import { alphanumeric } from '@nichoth/nanoid-dictionary';
```

### `nolookalikes`

Numbers and english alphabet without lookalikes: `1`, `l`, `I`, `0`, `O`, `o`, `u`, `v`, `5`, `S`, `s`, `2`, `Z`.

Complete set: `346789ABCDEFGHJKLMNPQRTUVWXYabcdefghijkmnpqrtwxyz`

```javascript
import { nolookalikes } from '@nichoth/nanoid-dictionary';
```

### `nolookalikesSafe`

Same as `nolookalikes` but with removed vowels and following letters: `3`, `4`, `x`, `X`, `V`.

This list should protect you from accidentally getting obscene words in generated strings.

Complete set: `6789BCDFGHJKLMNPQRTWbcdfghjkmnpqrtwz`

```javascript
import { nolookalikesSafe } from '@nichoth/nanoid-dictionary';
```
