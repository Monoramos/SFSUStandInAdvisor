# Transfer Advisor

## Privacy

Transcripts contain sensitive information, so privacy was a design
constraint from the start, not an afterthought.

**What this program does**
- **No storage.** Transcripts are processed in memory and discarded
  when the request ends. There is no user database, no file storage
  for uploads, and no accounts.
- **Minimal extraction.** The AI is asked for course code, title,
  units, grade, and term only. Name and student ID are not part of
  the extraction schema.
- **No content logging.** Application logs never include transcript
  contents or extracted courses.
- **Public data only in this repo.** Course, requirement, and club
  data come from public sources (see Data Sources). All sample
  transcripts are synthetic.

**What to know**
- The uploaded transcript is sent to Gemini on Google Cloud's
  Vertex AI for extraction, so it is subject to Google Cloud's
  data-handling terms. [VERIFY: link current terms and state
  retention accurately]
- The image may contain your name and ID when sent for processing,
  even though we don't extract them. [Remove if client-side
  redaction is built]

**Not official advice.** This is a planning aid. Always confirm
with your academic advisor and the official catalog.