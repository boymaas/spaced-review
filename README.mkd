# Spaced review

Spaced repetition is a learning technique that involves increasing the
intervals of time between reviewing previously learned material. The idea
behind spaced repetition is that reviewing material at increasingly longer
intervals helps to reinforce memory and improve retention of the material over
time.

This is a minimalistic, terminal-based tool for reviewing, scoring, and
storing retention information. It allows users to design their own method of
collecting and storing cards

## UNIX Philosophy

* Small is beautiful: Simple, small programs that do one thing well are
  preferred over complex programs that try to do many things.
* Make each program do one thing well: Programs should be designed to perform a
  single, well-defined task and do it well, rather than trying to do many
  things.
* Composability

Each user had individual needs and their own Philosophy on how to organize
their learning material.

## Features

* Cards and context are stored in files using the org-mode format.
* Learning progress is stored within the org-mode file.
* Configuration is done using command-line parameters, which can also be stored at the end of the org-mode file.
* Multiple files can be loaded together, or a whole directory can be reviewed. This allows you to use files as an easy way to group items (e.g. one file per level, one directory per domain, or one file per word class).
* The tool is written in Rust, which makes it fast and efficient.

## UX

We use the [TUI](https://github.com/fdehau/tui-rs)  to build our review interface.

## Usage

Install vocage using Rust's package manager:

```
cargo install spaced-review
```

## Based upon

* https://docs.rs/spaced-repetition/latest/spaced_repetition/#
  The algo implementing the spaced repetition algo

* https://github.com/PoiScript/orgize
  An org mode parser
