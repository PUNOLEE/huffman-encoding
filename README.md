# IPD Homework 8: Huffman Coding

## Summary

For this homework, you will write two programs:

  - `huff` compresses files using Huffman coding.

  - `puff` decompresses Huffman-coded files produced by `huff`, giving
    back the original file.

The filenames to read from and write to are passed to each program as
command-line arguments. For example, suppose you have a text file
`hamlet.txt` that you'd like to compress. You can compress it to a file
`hamlet.txt.huff` using your `huff` program:

```sh
    % ./huff hamlet-utf8.txt hamlet-utf8.txt.huff
```

You can decompress it using your `puff` program:

```sh
    % ./puff hamlet-utf8.txt.huff hamlet-utf8.txt.out
```

If you’ve done your job correctly, the decompressed file will match the
original. On UNIX (including Linux and Mac OS X) you can compare the two
to make sure they match using `diff`:

```sh
    % diff hamlet-utf8.txt hamlet-utf8.txt.out
```

When two files match, `diff` prints nothing.

