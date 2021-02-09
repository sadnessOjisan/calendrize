# calendarize

[![calendarize at crates.io](https://img.shields.io/crates/v/calendarize.svg)](https://crates.io/crates/calendarize)
[![calendarize at docs.rs](https://docs.rs/calendarize/badge.svg)](https://docs.rs/calendarize)

Just calendarize. This is imspired from Node.js [calendarize](https://github.com/lukeed/calendarize).

## how to use

```rs
let date = NaiveDate::parse_from_str("2021-01-02", "%Y-%m-%d").unwrap();
calendarize(date);

// [0, 0, 0, 0, 0, 1, 2],
// [3, 4, 5, 6, 7, 8, 9],
// [10, 11, 12, 13, 14, 15, 16],
// [17, 18, 19, 20, 21, 22, 23],
// [24, 25, 26, 27, 28, 29, 30],
// [31, 0, 0, 0, 0, 0, 0]
```

## development

```sh
# exec
cargo test
```
