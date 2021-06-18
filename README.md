> # ⚠️  TSLint [has been deprecated](https://blog.palantir.com/tslint-in-2019-1a144c2317a9) as of 2019. Please consider [migration to eslint](https://github.com/typescript-eslint/typescript-eslint).

# tslint-plugin-decorator-member-ordering

Extends `member-ordering` rule with decorators and Angular `ng` functions support.

Based on [PR#4202](https://github.com/palantir/tslint/pull/4202) created by [neilsoult](https://github.com/neilsoult).

## Installation

```sh
npm install --save-dev tslint-plugin-decorator-member-ordering
```

Then add plugin to `extends` property in your `tslint.json` file.

```json
{
    "extends": [
        ...,
        "tslint-plugin-decorator-member-ordering"
    ]
}
```

## Configuration example

```json
"decorator-member-ordering": [
    true,
    {
        "order": [
            "public-static-field",
            "protected-static-field",
            "private-static-field",

            "public-abstract-field",
            "protected-abstract-field",
            "private-abstract-field",

            "public-abstract-accessor",
            "protected-abstract-accessor",
            "private-abstract-accessor",

            "public-decorated-field",
            "protected-decorated-field",
            "private-decorated-field",

            "public-decorated-accessor",
            "protected-decorated-accessor",
            "private-decorated-accessor",

            "public-readonly-field",
            "protected-readonly-field",
            "private-readonly-field",

            "public-static-accessor",
            "protected-static-accessor",
            "private-static-accessor",

            "public-instance-field",
            "protected-instance-field",
            "private-instance-field",

            "public-instance-accessor",
            "protected-instance-accessor",
            "private-instance-accessor",

            "constructor",

            "ng-instance-method",

            "public-decorated-method",
            "protected-decorated-method",
            "private-decorated-method",

            "public-abstract-method",
            "protected-abstract-method",
            "private-abstract-method",

            "public-instance-method",
            "protected-instance-method",
            "private-instance-method",

            "public-static-accessor",
            "protected-static-accessor",
            "private-static-accessor",

            "public-static-method",
            "protected-static-method",
            "private-static-method"
        ]
    }
]
```
