---
title: A Sample Set of Slides
date: Totally Not the Last Minute
...

# An ordinary slide

With some text.

## And a block

And some text underneath.


::: note

Here are my notes.

:::

# Another slide

- With a
- list.
  - and sub item
    - and sub-sub item

::: notes

A note on my list.

:::

# A slide to show overlay tricks

\only<1,3>{This text appears on the first and third versions of the slide, but not the second.}

This uses beamer's highlighting command to \alert<2>{draw attention here}, but only on the second slide.

::: note<1>

Notes can also have overlay specs. First slide version note.

:::

::: note<2>

Second.

:::

::: note<3>

And third. Use markdown in notes: *emphasis*.

:::

# TeX-LOGO

\begin{textblock}{4}(0,1)
Grid demo UL
\end{textblock}

\begin{textblock}{4}(5,1)
\includegraphics[width=4\TPHorizModule]{tmp/figures/proj.pdf}
Grid demo UR
\end{textblock}
