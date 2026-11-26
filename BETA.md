# Local Training Studio private beta

Thank you for testing Studio. This takes about an hour, most of it waiting for downloads
and training. Please work through it on your own first, without help, and note where you
get stuck: that is the most useful thing you can tell us.

## Before you start

- Windows 10 or 11 with an NVIDIA GPU (any RTX card with 6 GB or more), a current driver,
  and about 20 GB of free disk space.
- Optional: [Ollama](https://ollama.com), to chat with the model you train.
- Please do not use confidential data during the beta unless you are allowed to. Studio
  keeps everything on your PC, but bug reports are seen by the Studio team.

## 1. Install (10–20 minutes)

1. Download the latest `LocalTrainingStudio-<version>.zip` from this repository's
   [Releases](https://github.com/GaneshShankaran-collab/local-training-studio/releases/latest) page, and extract it to a
   folder you will keep, such as `Documents\LocalTrainingStudio`.
2. Double-click **Install Local Training Studio.cmd**. If Windows shows "Windows protected
   your PC", click **More info → Run anyway** (the beta installer is not signed yet).
3. Studio opens in its own window when setup finishes. Note how long setup took.

If setup stops, it explains why. Fix the cause and run it again; it continues where it
stopped. If you cannot get past it, report it (step 7).

Studio walks you through four steps shown at the top: **Data → Model → Train → Test**.

## 2. The 5-minute demo

1. **Data:** click **5-minute demo**, then **Continue**.
2. **Model:** click **Start training** (if it says **Download**, click that first).
3. **Train:** watch the progress. When it finishes, Studio opens **Test** by itself.
4. **Test → How good is it?:** click **Score it**. You should see something like
   "50% → 100%, fixed 12 and broke none".

## 3. A free dataset

Click **New model** (top right), then **Free datasets**, and pick one from the top shelf (for
example *Bank customer questions → 77 intents*). Then **Continue**, and on the Model step
optionally **Check it** to see how the model does before training. Train, then score.

## 4. Your own task (the most important part)

Think of a repeated task from your work: routing tickets, tagging emails, pulling fields
out of text, rewriting notes in a house style. Put 20–200 examples in a spreadsheet with
one column for the input and one for the answer you want. Click **New model → Your
spreadsheet** and drop the file in (or paste the rows). If you have fewer than 50, click
**Draft examples**: read the drafts (they are marked **Draft**) and remove them if many look
wrong. Train, then score.

## 5. Try it with your own questions

In **Test → Try it**, type questions like the ones your team gets. You see the original model
and your trained model answer side by side.

## 6. Use it

In **Test → Use it**: **Add to Ollama**, then pick where you want to use it (a terminal, the
GitHub Copilot app, VS Code, or your own app) and follow the steps. **Check the connection**
confirms it works.

## 7. Tell us how it went

- **Feedback:** **Help → Send feedback** opens a short form (about 5 minutes). Two questions
  matter most to us: how disappointed you would be without Studio, and what you would pay for.
- **Problems:** **Help → Save diagnostics** creates a ZIP with Studio's version, your GPU and
  driver, and recent logs, and opens its folder. It contains no datasets, examples, prompts,
  answers or models. Attach it to a problem report.
- **Usage statistics:** Studio asks once whether you will share anonymous usage statistics
  (which steps you use, timings, model names, errors; never your data). Saying yes during the
  beta helps a lot. **Help → Usage statistics** shows exactly what is sent; see TELEMETRY.md.
