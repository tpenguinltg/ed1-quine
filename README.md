# ed(1) Quine

***[Quine][]:** A program that produces its own source code as output.* ([Wiktionary][wiktionary-quine])

[Quine]: https://en.wikipedia.org/wiki/Quine_%28computing%29
[wiktionary-quine]: https://en.wiktionary.org/wiki/quine#Noun

This ed(1) script, when run through `ed` with no file, will print its own source code.

## Running

```
$ ed < quine.ed
```

The filename of the script is not important. The script does not even have to be in a file.

### Verifying

```
$ ed < quine.ed > quine.out
$ diff quine.ed quine.out
```

The `diff` should produce no output and exit with success (0).

## License

MIT. See the [LICENSE][] file for details.

[LICENSE]: LICENSE
