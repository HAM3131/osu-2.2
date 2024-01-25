# Lecture 10 - Redirection
In Linux/Unix there are 3 file descriptors explicitly defined for 3 distinct datastreams:
 - `stdin` (0)
 - `stdout` (1)
 - `stderr` (2)

We can change the destination of these data streams from the command line with any of the following:
 - `<` redirects input
 - `>` redirects output
    - `>>` appends if file already exists
 - `2>` redirects errors
