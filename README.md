# Local Training Studio

**Run, compare and teach local AI models on your own PC: chat with any model, ask your documents,
train a model on your task with proof that it got better, train video styles, and use it all in the
GitHub Copilot app, VS Code or your own app.** No code, no cloud: your data never leaves your machine.

This repository holds Studio's **releases and documentation**. Download the app from
[Releases](https://github.com/GaneshShankaran-collab/local-training-studio/releases/latest).

## Install

1. Download the latest **LocalTrainingStudio-&lt;version&gt;.zip** from
   [Releases](https://github.com/GaneshShankaran-collab/local-training-studio/releases/latest) and
   extract it to a folder you will keep, such as `Documents\LocalTrainingStudio`.
2. Double-click **Install Local Training Studio.cmd**. The first install downloads about 3.2 GB and
   takes 10–20 minutes. If Windows shows "Windows protected your PC", click **More info → Run
   anyway** (beta builds are not code-signed yet).
3. Studio opens in its own window with three areas: **Chat**, **Models** and **Train**.

**Linux and macOS:** extract the ZIP and run `bash install.sh`. Then open Studio with `./studio-app`
(Linux also gets an applications-menu entry; on a Mac, double-click `Local Training Studio.command`).
Use it from a terminal with `./studio --help`.

**Needs:** Windows 10 or 11, Linux (Ubuntu 22.04 or newer tested) or macOS, and Python 3.10+ on Linux
and macOS. Chat, Models, documents, pictures and tools work on any recent PC or Mac; Studio's engine
uses CUDA, Vulkan (any GPU), Apple Metal or the CPU. Training needs an NVIDIA GPU with 6 GB or more, on
Windows or Linux; training on a Mac is not available yet.

**Update:** from 0.9.5 on, Studio checks for new versions when it opens and every hour, shows them
in a banner, and installs them by itself as it opens (Help → Software Update to turn that off).
**Update Now** installs and restarts straight away. Your models, runs and data are always kept.
Older versions are marked *Deprecated* on the releases page. To update by hand, extract a newer
ZIP over your install folder and run the installer again.

## What you can do

**Chat and Models**

- **Chat** with any local model, with streaming answers, code blocks, speed per answer, Regenerate,
  Edit and Export. **Compare** two models side by side on the same messages.
- **Ask your documents:** attach PDFs, Word files and code; answers cite the file and page.
- **Pictures:** show pictures to models that can see, such as Gemma 3.
- **Models:** see what is installed and in memory and how each fits your GPU; download hand-picked
  models or any GGUF model from Hugging Face.
- **Studio's own engine** (llama.cpp): runs your model files directly, including models Ollama already
  downloaded, on Windows, Linux and macOS. Ollama is optional.
- **Tools:** models can use a clock, an exact calculator, Studio's video tool and any MCP server; anything
  that acts asks you first. JSON and schema answers, presets, and a command line (`studio`).

**Train your own model**

- **Data:** start from free datasets that allow commercial use, your own CSV or Excel file, or a
  5-minute demo. Studio checks the data and can draft more examples in your style.
- **Model:** Studio picks the strongest model that fits your graphics card.
- **Train:** live progress, time left and learning curves.
- **Test:** ask your own questions to the original and the trained model side by side, and get a
  before-and-after score on examples the model never saw.
- **Use it:** add it to Ollama, then follow the steps for a terminal, the GitHub Copilot app,
  VS Code, or your own app, and check the connection.

**Train a video style (Wan 2.1)**

- Give Studio a folder of short clips with captions; it trains a video LoRA on your GPU, shows
  before-and-after videos, and adds a **make_video** tool to the GitHub Copilot app so you can ask
  for videos in your style. Video needs about 16 GB of free graphics memory and a one-time
  download of about 19 GB.

## Beta testers

Start with [BETA.md](BETA.md). Send feedback privately from Studio's **Help → Send Feedback**.
Issues here are **public**: report problems with the **Problem report** or **Beta feedback** form,
and leave out private data.

## Privacy

Your examples, prompts and answers never leave your PC. Studio goes online only to download
models, the datasets you choose, and updates. If you agree when Studio asks, it also sends
anonymous usage statistics, never your data. See [TELEMETRY.md](TELEMETRY.md).

## License

[MIT](LICENSE). Models you download and train keep their own licenses, which Studio shows.
