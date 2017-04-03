This is a benchmark between multiple programs doing the task specified
[here](https://github.com/d-muc/clean-code-competition17/tree/master/task1) (without
file and argument parsing).

Executing `run.sh` builds the programs (with release profile) and then benchmarks them
with Rust's integrated bencher.

As Rust's integrated bencher is unstable, a nightly toolchain is required. Recommended
installation method is obtaining [rustup.rs](https://rustup.rs/) (a Rust toolchain manager) and
running `rustup override add nightly` in this directory.

More versions are welcome! Just send a pull request. I can take care of adding it to the benchmark.

Credits:
- Rust version by me (Bobo1239)
- D version by [Stefan](https://www.meetup.com/Munich-D-Programmers/members/184727568/)

## Bonus Round

With `test.large` which is 370 Mb and not included in this repository.
Only tested with a simple `time cat test.large | <prog>`.

- Rust: 1.168s
- D (dmd): 4.952s