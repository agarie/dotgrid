# dotgrid
a web app to generate dot-grid pdfs

This is a simple javascript application that generates a PDF side on the client
side for either one or two pages of dot grid.

While the "interface" should be perfectly functional, there has been no effort
to make it aesthetically pleasing. PRs beautifying the app are welcomed.

The output contains no watermarks or other such nonsense (a major problem with
many dot-grid generators online), so if you find it useful star the project or
post something on social media or otherwise just spread good vibes, man.

Carlos: I made a few changes to this repo to add features I wanted, and changed
the defaults to something closer to what I personally use. Thanks to rvcx!

## References

Carlos: I used the following resources when trying to understand the syntax in
order to make changes to this repo. There's nothing particular complicated
about the stuff in this repo, but it's good to have a stronger idea of what's
going on. Feel free to add more refs or summarize things if that makes sense.

- Adobe PDF Reference 1.4 (PDF): https://opensource.adobe.com/dc-acrobat-sdk-docs/pdfstandards/pdfreference1.4.pdf
- ISO 32000-2 (PDF 2.0): https://developer.adobe.com/document-services/docs/assets/5b15559b96303194340b99820d3a70fa/PDF_ISO_32000-2.pdf
- PDF Association Cheat Sheet (PDF): https://pdfa.org/wp-content/uploads/2023/08/PDF-Operators-CheatSheet.pdf
- PDF Syntax (ISO 32000-2): https://pdf-issues.pdfa.org/32000-2-2020/clause07.html
- PDF Explained (GitHub): https://github.com/zxyle/PDF-Explained
- PDF Syntax Guide: https://pdf-issues.pdfa.org/32000-2-2020/clause08.html

A few operators:

| Operator | Description |
|----------|-------------|
| m | Move to (start path) |
| l | Line to |
| c | Cubic Bézier curve |
| re | Rectangle (x y width height re) |
| f | Fill path |
| s | Stroke path |
| S | Stroke and close path |
| q | Save graphics state |
| Q | Restore graphics state |
| cm | Current transformation matrix |
| w | Set line width |
| g | Set grayscale fill color |
| G | Set grayscale stroke color |
