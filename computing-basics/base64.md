# Base 64

A binary-to-text encoding is a way of taking binary data and turning it into
text so it's more safely transmitted across text channels such as email or HTML
form data.

8-bit clean describes a computer system that correctly handles 8-bit character
encodings, such as UTF-8 encoding of Unicode.

Till the early 1990s many programs and data transmission channels assumed that
all characters would be represented as numbers between 0 and 127 (7 bits). The
8th bit of an 8-bit byte was sometimes used as a control bit.

Some transmission channels have 7 bits per byte and some have 8 bits. 7 bit
channels are made for streaming text and can transfer ASCII text only. Binary
files cannot be transmitted through 7-bit data channels directly because some
protocols may interpret certain sequences as control characters. SMTP (without
extensions) is a 7 bit channel, and SMS is another.

The bits in a text file represent characters whereas the bits in binary
represent custom data understood by the running program.

Passing the `b` argument when opening a file indicates that the file contains
binary as opposed to text data, and so not to rewrite characters.

```ruby
File.open(<filename>, "wb")
```

There are different conventions for line-endings and text-transmission channels
will convert these line-endings automatically. A binary file would get mangled.

To safely transfer a binary file is must be encoded using a binary-to-text
encoding system. Base64 is one such encoding.
