# trb -- Textus Receptus on the Command Line

A command line tool for search and reading the Bible in Greek.
This is the Textus Receptus (Scrivener 1894).

Format and original implementation from [bontibon/kjv](https://github.com/bontibon/kjv).

## Usage

    usage: ./trb [flags] [reference...]

      -l      list books
      -W      no line wrap
      -h      show help

      Reference types:
          <Book>
              Individual book
          <Book>:<Chapter>
              Individual chapter of a book
          <Book>:<Chapter>:<Verse>[,<Verse>]...
              Individual verse(s) of a specific chapter of a book
          <Book>:<Chapter>-<Chapter>
              Range of chapters in a book
          <Book>:<Chapter>:<Verse>-<Verse>
              Range of verses in a book chapter
          <Book>:<Chapter>:<Verse>-<Chapter>:<Verse>
              Range of chapters and verses in a book

          /<Search>
              All verses that match a pattern
          <Book>/<Search>
              All verses in a book that match a pattern
          <Book>:<Chapter>/<Search>
              All verses in a chapter of a book that match a pattern




## Build

trb can be built by cloning the repository and then running make:

    git clone https://github.com/VBotkin/trb.git
    cd trb
    make

## License

Public domain
