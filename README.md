# PNGCrush.html
Really good PNG compressor web application. It is 2,500KB of JavaScript ByteCode compressed to about 250KB in a self extracting and auto executing HTML file. 

Enable reuse by page refresh, sorry but for multiple files it's not setup well, but for one or 2 quick reductions for performance gain, it rocks and does the job better than any paid software!

Source code used: https://github.com/richardassar/pngcrush.js
It is an optimizer for PNG (Portable Network Graphics) files, ported to JavaScript with Emscripten for use in the browser.

Live demos:

http://codepen.io/samples/pen/WQNbVr

http://jsfiddle.net/mqezaknv/

MORE TECH DETAILS:

pngcrush is a free utility for optimizing PNG image files. It reduces the size of the file losslessly — that is, the resulting "crushed" image will have the same quality as the source image. The main purpose of pngcrush is to reduce the size of the PNG IDAT data stream by trying various combinations of compression methods and delta filters. It can also be used for various manipulations of PNG images, such as changing the bit depth, removing unwanted ancillary chunks, or adding certain chunks including gAMA, tRNS, iCCP, and textual chunks. The pixel data in a PNG file is compressed using LZ77 algorithm (which tries to find repeated byte sequences in the source data), and then further compressed with Huffman algorithm. This combination is referred to as DEFLATE compression. Before compressing, non-destructive delta filters are applied on the pixel data. There are 5 possible filter types that can be specified separately on each scan line and several possible strategies for searching LZ77 matches. Thus, there are a very large number of different combinations for how the image can be compressed. Which combination gives the best compression will depend on the individual image's properties. pngcrush compresses the image with multiple different combinations and then stores the smallest of the resulting files. Since it is not possible to go through all the combinations, pngcrush uses heuristics to choose the methods to try. Since most graphics software embed the extra color-correction data, which is normally not needed, removing it can produce file sizes that are up to 40% smaller than the original. pngcrush, when told, will also losslessly reduce the bit-depth of images or apply a color palette when possible if doing so results in a smaller file size.
