# Repeat Effect

Repeat a parsed Skript effect a fixed number of times without writing a separate loop block.

## Requirements

- Skript 2.15+
- skript-reflect 2.6+

## Installation

```
package install https://github.com/devdinc/repeat-effect
```

## Syntax

```skript
[repeat] <effect> once
[repeat] <effect> twice
[repeat] <effect> thrice
[repeat] <effect> %number% times
```

The effect is parsed once and then executed the requested number of times in the current event.

## Examples

```skript
repeat broadcast "Hello" thrice

repeat add 1 to {_count} five times

broadcast "This happens once" once
```

The number of executions is determined by the selected quantity. A numeric quantity can be supplied as an expression.

## Source and tests

- Implementation: `src/repeat-effect.sk`
- Tests: `-tests/`
