# John Crenshaw

Software engineer. I build things when the existing answer is missing, unreliable, or more complicated than the problem deserves.

Most of my current work is in Rust, Linux, and AI-assisted software engineering.

## AI-assisted engineering

### [Cadence](https://github.com/crenshawdev/cadence)

An engineering methodology for Claude Code, for code that has to keep working after you ship it.

The model can plan, build, and review. The controls around it make sure checks actually run, failures stay visible, and the thing that produced the work is never solely responsible for certifying it.

Cadence is the clearest expression of how I think about AI-assisted development: automation is useful, but appearance is cheap. Verification is the work.

### [Terminus](https://github.com/crenshawdev/terminus)

Persistent, cross-session memory for Claude Code built on one premise: the transcript is the record.

Terminus keeps the original session intact and builds retrieval on top of it. Nothing is summarized away on ingest; indexes and observations are derived data that can be rebuilt from the source.

Still in development.

### [burnrate](https://github.com/crenshawdev/burnrate)

A local, on-demand dashboard for Claude Code usage.

It reconstructs token usage from local transcripts by project, model, command, session, and rate-limit window, then produces a self-contained HTML report. No network calls. No telemetry. No account.

## GUI

### [Tempest](https://github.com/crenshawdev/tempest)

A weather applet for the COSMIC desktop with current conditions, hourly and 7-day forecasts, a 24-hour meteogram, weather alerts, air quality, multiple locations, and regional data sources.

It is also where a lot of my desktop work shows up: application structure, state, asynchronous data, internationalization, networking, packaging, and the less glamorous parts of GUI software that determine whether it still works six months later.

## Rust & Linux systems

### [weathervane](https://github.com/crenshawdev/weathervane)

The Rust library underneath Tempest.

It handles weather, air quality, pollen, alerts, location, network state, units, and provider differences, then hands the frontend clean Rust types. No UI dependencies, polling framework, or configuration layer. The application owns those decisions.

### [PowerCurve](https://github.com/crenshawdev/powercurve)

A Linux power-management daemon compatible with `power-profiles-daemon`, with optional hwmon fan control, configurable curves, hysteresis, and thermal protection.

It is deliberately a desktop and workstation tool: power policy and hardware control without pretending every machine exposes the same mechanisms.

## Writing

I write about software engineering, AI, open source, and the decisions underneath the code at [jcrenshaw.dev](https://jcrenshaw.dev/writing).

**Appearance is cheap. Verification is the work.**
