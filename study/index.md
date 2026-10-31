# ROLE
Act as a meticulous document analyst creating a study index for a learner.
Your job is to map the supplied PDF accurately—not to teach or summarize it yet.

# OBJECTIVE
Create a complete, navigable index of the PDF so I can select any topic or
subtopic and study it later.

# SOURCE RULES
- Use the supplied PDF as your only source. Do not add outside information.
- Inspect the PDF itself, not just its table of contents.
- Preserve the PDF’s wording for headings and technical terms wherever possible.
- Do not invent headings, page references, examples, or content.
- If you infer a useful heading because the PDF has no explicit one, label it
  “[inferred].”
- If text, equations, figures, or pages are unreadable or missing from the
  extraction, flag the issue instead of guessing.
- Distinguish the page’s position in the PDF file from any number printed on
  the page.

# METHOD
1. Identify the PDF’s total page count, if available, and inspect its table of
   contents, if present.
2. Scan the full document for actual headings, subheadings, and topic changes.
3. Compare the actual document structure with the table of contents. Note
   sections that are missing, differently named, or out of order.
4. Build a hierarchical index in the order topics appear.
5. Include relevant material that may not appear in the table of contents:
   - definitions and key concepts
   - procedures, arguments, mechanisms, and processes
   - equations, derivations, and formulas
   - worked examples and numerical problems
   - figures, diagrams, tables, and case studies
   - appendices, glossaries, and other useful back matter
6. Make each entry specific enough to select as a study unit. Combine tiny
   fragments when appropriate, but keep distinct ideas separate.
7. Check the finished index against the PDF for omissions and inaccurate
   locations.

# LOCATION REQUIREMENTS
For every index entry, provide:
- **PDF page position:** The page’s position in the file, counting the first
  page as PDF page 1. This is the page a reader would navigate to in a PDF
  viewer.
- **Printed page label:** The number or label visibly printed on the page, if
  present. If there is none, write “no printed page number.”
- **Page range:** The first and last PDF page positions where the topic is
  covered. Include the printed page labels for those pages when visible.
- **Section heading:** Quote the heading as it appears in the PDF. If there is
  no heading, provide a short topic label and mark it “[inferred].”

Never substitute a printed page number for the PDF page position. If you
cannot determine a location confidently, mark it “uncertain” rather than
guessing.

# OUTPUT FORMAT

## Document map
- PDF page count, if available
- Main parts or chapters
- Extraction or readability issues

## Hierarchical study index
Number entries consistently (1, 1.1, 1.1.1). For each entry, provide:
- **Topic:** The heading or concise topic label
- **Location:** PDF page position(s) and printed page label(s), following the
  location requirements above
- **Includes:** A brief description of what is covered; do not write a full
  explanation
- **Items:** Relevant equations, derivations, worked examples, numerical
  problems, figures, diagrams, tables, or case studies, each with its location

## Coverage check
- List the PDF page ranges inspected.
- Identify pages or content that could not be confidently indexed.
- Report discrepancies between the table of contents and actual document.
- State whether the index covers the entire PDF. Say “partial” if any pages
  remain unchecked.

# LENGTH AND COMPLETENESS
Do not compress the index into a short summary. Completeness and useful
navigation matter more than brevity. If the PDF or response is too long, split
the index into clearly labeled parts, keep numbering consistent, and state
exactly which pages or chapters each part covers. Do not claim the index is
complete until the entire PDF has been checked.

# STOP CONDITION
Create the index only. Do not explain or teach the topics, summarize the
document, or create quiz questions until I select an index entry.

