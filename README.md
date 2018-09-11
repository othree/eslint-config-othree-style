# eslint-config-othree-style

* [semistandard][] + [trailing comma][comma-dangle] on multiline
* [eslint-plugin-no-parameter-e][]
* [eslint-plugin-pep8-blank-lines][]

## Why

I love standardjs and semistandard. But I really want trailing comma.

Trailing Comma is not allowed in old JavaScript implementations.
But for a long list with tailing comma is easier to maintain.

It's easier to modify a list since every element are in the same format.
Reduce the chance produces bug when copy element from old code.

Also, minifier can strip trailing commas, so don't worry about old browsers.

## Other Rules

My custom rules:

* [eslint-plugin-no-parameter-e][].
* [eslint-plugin-pep8-blank-lines][]

## Usage

Because deps are based on peerDependency. We need to install all eslin config ourself.

```sh
npm install --save-dev \
  eslint-config-othree-style \
  eslint-config-standard \
  eslint-plugin-standard \
  eslint-plugin-promise \
  eslint-plugin-import \
  eslint-plugin-node \
  eslint-plugin-no-parameter-e \
  eslint-plugin-pep8-blank-lines
```

Add this to esling config:

```json
{
  "extends": "othree-style"
}
```

[semistandard]:https://github.com/Flet/semistandard
[comma-dangle]:https://eslint.org/docs/rules/comma-dangle
[eslint-plugin-no-parameter-e]:https://github.com/othree/eslint-plugin-no-parameter-e
[eslint-plugin-pep8-blank-lines]:https://github.com/othree/eslint-plugin-pep8-blank-lines
