# phpstorm-repro

This repository is a more or less minimal reproduction of an issue, where PhpStorm is unable
to resolve the type of generic components when passing function arguments.

The type of the `result` property of the default slot of the `GenericComp` component in `App.vue`
is not resolved, whereas VSCode with Volar is capable of doing so.