# OffLadder: career change coach for Claude

OffLadder helps people change careers in small tests instead of guesses. This plugin teaches Claude OffLadder's method for testing a career before committing, finding directions that fit, tailoring a CV and cover letter to a job, answering application questions, preparing for interviews, negotiating offers, returning to work after a break and planning the month after a layoff. It also connects Claude to OffLadder's no-login connector, which searches more than 300 written, sourced career guides.

Made by [OffLadder](https://offladder.com), whose AI coach Laddie helps people find two directions worth testing and try a real piece of the work.

## Install

- **Claude (web, desktop and Cowork)**: open the directory, search for OffLadder and add the plugin.
- **Claude Code**: `/plugin install offladder --marketplace wonderwhiz/offladder-claude`

## What's inside

### Skills (16)

| Skill | Use it when you want to… |
| --- | --- |
| `test-a-career` | try a career with a small real-world experiment before you quit anything |
| `find-career-directions` | find two or three directions worth testing when you don't know what you want |
| `plan-a-career-change` | plan a career change at any age, without quitting first or retraining blindly |
| `tailor-cv-to-job` | tailor your CV or resume to a job description, honestly and ATS-friendly |
| `write-cover-letter` | write a short cover letter for one specific job |
| `answer-application-questions` | draft answers to application form and screening questions |
| `prepare-for-interview` | prepare likely questions, STAR stories and "tell me about yourself" from the job post |
| `after-a-layoff` | make a calm 30-day plan after a layoff or redundancy |
| `future-proof-against-ai` | see how AI changes your job task by task, and what to move towards |
| `informational-interviews` | reach out to people in a field and run an informational interview |
| `follow-up-on-applications` | follow up after applying or interviewing, and track applications |
| `choose-a-path-as-a-student` | choose a major, degree route, apprenticeship or first job |
| `negotiate-a-job-offer` | research pay, answer the salary question, negotiate or compare offers |
| `return-to-work-after-a-break` | come back to work after caring, illness, study or a long break |
| `update-linkedin-for-a-career-change` | rewrite your LinkedIn headline and About section for the job you want |
| `start-a-new-job` | get through the first week, first payslip and probation |

Skills load on their own when your question needs one. In Claude Code you can also call one directly, for example `/offladder:tailor-cv-to-job`.

### The OffLadder connector

The plugin adds OffLadder's remote MCP server at `https://offladder.com/claude/mcp`. It needs no account or sign-in, and every tool is read-only:

- `find_career_experiment`: one small experiment to test a named career this week
- `explore_career_directions`: emerging kinds of work that fit what someone enjoys, each with a test
- `find_career_guide`: searches OffLadder's career guides (career changes, layoffs, AI and jobs, degrees, CVs and resumes, cover letters, applications, interviews)
- `read_career_guide`: the full text of one guide, with its sources
- `browse_career_guides`: every guide on one subject, such as CVs and applications, layoffs, interviews and pay, or students and first jobs
- `get_career_direction`: one of OffLadder's emerging directions of work in full, or the list of all of them
- `check_career_change_facts`: exact quotes from the U.S. Bureau of Labor Statistics, O*NET and the World Economic Forum
- `start_my_reading`: a link to OffLadder's short onboarding

## Things to ask

- "I'm a teacher thinking about UX design. How could I test it this weekend?"
- "Here's a job post and my CV. Tailor my CV to it without making anything up."
- "Is it too late to change careers at 45?"
- "I was laid off yesterday. What should I do this month?"
- "Help me prepare for my interview on Thursday. Here's the job description."
- "Will AI take my job as a paralegal?"
- "They offered me £45k. How do I ask for more?"
- "I've been home with my kids for six years. How do I go back to work?"

## What this plugin runs, sends and stores

- The skills are instructions for Claude only. They run no code and send nothing anywhere.
- When Claude uses an OffLadder tool, it sends `https://offladder.com/claude/mcp` only the words it chose for that question, such as a career name or a short question. The tools read OffLadder's published pages; they don't sign you in, read or change an OffLadder account, call an AI model, or store what was sent, apart from the short-lived request logs our hosting provider keeps for every page.
- Links in the answers carry `utm_source=claude` so OffLadder can count visits from Claude. If you open one, offladder.com works as its privacy policy describes.
- Nothing reads your files, your other conversations or Claude's memory.

Privacy policy: https://offladder.com/privacy · Documentation: https://offladder.com/claude

## Good to know

Directions and experiments are possibilities to test, not a verdict on you. OffLadder is a coach, not a qualified careers, legal or financial adviser. It is for ages 13 and up.

## Support

Email hello@offladder.com with the question you asked and what went wrong.

## License

MIT. See [LICENSE](LICENSE).
