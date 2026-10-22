# GOAL Finance – Broker Recruitment Survey

Single-page, survey-style landing page (`index.html`) for recruiting mortgage brokers into the GOAL Broker Success System. No build step – open the file or host it on any static host.

## Collecting submissions

Set `SUBMIT_URL` near the top of the `<script>` in `index.html` to a webhook (Make, Zapier, CRM). Answers are POSTed as JSON:
`firstName, stage, challenges[], help[], timeframe, email, phone, source, submittedAt`.

With `SUBMIT_URL` empty the survey still runs and shows the thank-you screen, but nothing is sent.

## Editing

- Questions/options: the `steps` array in the script.
- Colours: CSS variables in `:root` (`--accent` is the button/progress colour).
