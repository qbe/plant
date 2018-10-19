# plant

A command line utility for visualization of hirarchical data in tree form,
written in python and thus portable to pretty much anything.

The program "plant" will read in any number of lines, and arrange them internally
in an n-ary tree, where each line is broken up into "identifiers" and "seperators",
with the "seperators" specifiable via the argument "-r REGEX".

After the program receives the end-of-file signal or runs over the configured
threshhold of objects in the tree, it will start printing the tree in a visually
pleasing and configurable manner.

The input should be in depth-first traversal manner(e.g. child items should come before
siblings), which is automatically done by pretty much any recursively working utility.
Lexically sorting the input lines is not necessary, but will accomplish the depth-first
traversal requirement for any input.

The difference of this program compared to the canonical utility "tree" is that it
* works on any dataset and is not limited to file paths
* works on piped input and can thus display filtered and/or modified input
* has a lot of visual options, including indent length, line style, and folding

# installation

Just copy the file to your computer. If you have Python 3 installed it should work out
of the box. If you want to be able to run it as any command line utility, copy it to
a location in your $PATH. Packages for Arch Linux are avaliable via the AUR, packages
for different distributions are to be done.
