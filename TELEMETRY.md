# Usage statistics

Studio can send **anonymous, opt-in usage statistics** so the team can see which steps people
use, where they get stuck, and what fails. This page says exactly what is collected, and how
the team turns on the dashboards.

## For people using Studio

- **Off until you say yes.** The first time Studio opens, it asks. Change your answer any time
  under **Help → Usage statistics**, which also lists the events waiting to be sent and the last
  ones sent.
- **Anonymous.** Each install has a random ID. No name, email, account, or location from your IP
  address (Studio asks the service not to look it up).
- **No content, ever.** Never your examples, prompts, answers, file or dataset names, paths, or
  anything you type.
- **Turn it off for a whole PC** by setting the environment variable `STUDIO_TELEMETRY=0`.

What each event can contain:

| Event | When | Fields (besides the event name) |
|---|---|---|
| `app_started` | Studio opens | version |
| `data_chosen` | Examples are prepared | source (library, import, demo), examples, test_examples, scoring |
| `drafted` | Write more examples finished | count |
| `base_checked` | The base model was checked | profile, before, total |
| `training_finished` | Training ended | profile, status, steps, minutes |
| `compared` | Scoring finished | kind (better, mixed, same, worse), before, after, total |
| `test_asked` | A question in Try it | (none) |
| `exported` / `export_failed` | Use it → Add to Ollama | quantization, profile |
| `use_checked` | Check the connection | (none) |
| `shared` | A result card was made | (none) |
| `crash` | An unexpected error | kind (the error type, for example `ValueError`) |
| `rated` | 👍 or 👎 on "Was this useful?" | score (1 or 0), where (score, try, use) |
| `step_viewed` | A step was opened | step |
| `destination_viewed` | A Use it destination was opened | destination |

Every event also carries: Studio's version, the Windows version, and a GPU size class such as
"up to 16 GB".

### Private feedback (Help → Send Feedback)

This is separate from the usage statistics above, and nothing is sent until you press
**Send Privately**. It sends your answers to the feedback questions (how useful Studio was, what
you would pay for and how much, whether your team would use it, your real task, what was
confusing, and a way to reach you if you give one), together with Studio's version, the Windows
version, the GPU size class, the random install ID and the minutes to your first result. It goes
to the same private service the Studio team uses for usage statistics, never to a public page.
Please leave out private or customer data. Problem reports on GitHub, by contrast, are public.
