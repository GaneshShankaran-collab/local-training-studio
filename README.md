# Local Training Studio

**Teach a local AI model your task on your own PC, see proof that it got better, and use it
anywhere: Ollama, the GitHub Copilot app, VS Code, or your own app.** No code, no cloud: your
examples never leave your machine.

This repository holds Studio's **releases and documentation**. Download the app from
[Releases](https://github.com/GaneshShankaran-collab/local-training-studio/releases/latest).

## Install

1. Download the latest **LocalTrainingStudio-&lt;version&gt;.zip** from
   [Releases](https://github.com/GaneshShankaran-collab/local-training-studio/releases/latest) and
   extract it to a folder you will keep, such as `Documents\LocalTrainingStudio`.
2. Double-click **Install Local Training Studio.cmd**. The first install downloads about 3.2 GB and
   takes 10–20 minutes. If Windows shows "Windows protected your PC", click **More info → Run
   anyway** (beta builds are not code-signed yet).
3. Studio opens in its own window and walks you through four steps: **Data → Model → Train → Test**.

**Needs:** Windows 10 or 11, an NVIDIA RTX GPU with 6 GB or more, a current driver, and about 20 GB
of free disk space. Optional: [Ollama](https://ollama.com), to use your model in other apps.
Mac and AMD GPUs are not supported yet.

**Update:** from 0.9.5 on, Studio checks for new versions when it opens and every hour, shows them
in a banner, and installs them by itself as it opens (Help → Software Update to turn that off).
**Update Now** installs and restarts straight away. Your models, runs and data are always kept.
Older versions are marked *Deprecated* on the releases page. To update by hand, extract a newer
ZIP over your install folder and run the installer again.

## What you can do

- **Data:** start from free datasets that allow commercial use, your own CSV or Excel file, or a
  5-minute demo. Studio checks the data and can draft more examples in your style.
- **Model:** Studio picks the strongest model that fits your graphics card.
- **Train:** live progress, time left and learning curves.
- **Test:** ask your own questions to the original and the trained model side by side, and get a
  before-and-after score on examples the model never saw.
- **Use it:** add it to Ollama, then follow the steps for a terminal, the GitHub Copilot app,
  VS Code, or your own app, and check the connection.

## Beta testers

Start with [BETA.md](BETA.md). Send feedback and report problems from Studio's **Help** menu, or
open an issue here with the **Beta feedback** or **Problem report** form.

## Privacy

Your examples, prompts and answers never leave your PC. Studio goes online only to download
models, the datasets you choose, and updates. If you agree when Studio asks, it also sends
anonymous usage statistics, never your data. See [TELEMETRY.md](TELEMETRY.md).

## License

[MIT](LICENSE). Models you download and train keep their own licenses, which Studio shows.
