
# Erlang quickstart

How Erlang projects are usually set up and checked. Always prefer the project's own `CONTRIBUTING.md` when it says something different.

Open Erlang issues: [Erlang issue list](../issues/by-language/erlang.md)

## Setup

- Install Erlang/OTP and Rebar3 using the official installation instructions.
- Check `.tool-versions`, the project README, and CI configuration for the required Erlang/OTP version.
- Check `rebar.config` for dependencies, plugins, and project-specific settings.

## Common commands

| Task | Usual command |
| --- | --- |
| Check Erlang/OTP version | `erl -version` |
| Check Rebar3 version | `rebar3 version` |
| Compile the project | `rebar3 compile` |
| Run EUnit tests | `rebar3 eunit` |
| Run Common Test suites | `rebar3 ct` |
| Check formatting | `rebar3 fmt --check` (when configured) |
| Format the project | `rebar3 fmt` (when configured) |
| Run Dialyzer checks | `rebar3 dialyzer` (when configured) |

## Tips

- Use the Erlang/OTP version specified by the project, especially when `.tool-versions` is present.
- Rebar3 commands depend on the project's configuration and installed plugins. Check `rebar.config` and CI before running them.
- Formatting commands require a configured formatter plugin. Follow the project's own instructions if it uses `erlfmt` or another formatter.
- Dialyzer checks may require PLT files and project-specific configuration.

## Before you push

- [ ] Tests for the area you changed pass locally.
- [ ] Formatter and linter pass with the project's configuration.
- [ ] Your diff contains no unrelated formatting or lockfile changes.

Back to [all languages](README.md) · [Guide](../guide/README.md)
