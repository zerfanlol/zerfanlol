<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Terminal OS</title>
  <style>
    :root {
      --bg: #0d0f12;
      --fg: #8b949e;
      --accent: #c9d1d9;
      --dim: #484f58;
      --prompt: #6e7681;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      background-color: var(--bg);
      color: var(--fg);
      font-family: "Courier New", Courier, monospace;
      font-size: 14px;
      line-height: 1.4;
      padding: 20px;
      height: 100vh;
      overflow-y: auto;
    }

    /* Эффект ЭЛТ-монитора / Старого экрана */
    body::before {
      content: " ";
      display: block;
      position: fixed;
      top: 0; left: 0; bottom: 0; right: 0;
      background: linear-gradient(rgba(18, 16, 16, 0) 50%, rgba(0, 0, 0, 0.25) 50%);
      background-size: 100% 4px;
      z-index: 10;
      pointer-events: none;
      opacity: 0.6;
    }

    #terminal {
      max-width: 900px;
      margin: 0 auto;
    }

    .output-line {
      white-space: pre-wrap;
      word-break: break-all;
      margin-bottom: 4px;
    }

    .ascii-art {
      color: var(--accent);
      font-weight: bold;
    }

    .info-key { color: var(--accent); font-weight: bold; }
    .info-val { color: var(--fg); }

    .input-line {
      display: flex;
      align-items: center;
      margin-top: 8px;
    }

    .prompt {
      color: var(--prompt);
      margin-right: 8px;
      user-select: none;
    }

    input {
      background: transparent;
      border: none;
      color: var(--accent);
      font-family: inherit;
      font-size: inherit;
      flex: 1;
      outline: none;
    }

    .colors-bar span {
      display: inline-block;
      width: 12px;
      height: 12px;
      margin-right: 4px;
    }
  </style>
</head>
<body>

<div id="terminal">
  <div id="history"></div>
  <div class="input-line">
    <span class="prompt">user@wired:~$</span>
    <input type="text" id="cmdInput" autofocus spellcheck="false">
  </div>
</div>

<script>
  const history = document.getElementById('history');
  const input = document.getElementById('cmdInput');

  // ASCII Арт картинки для fastfetch (Lain / Monochome aesthetic)
  const asciiPic = `
       .---.      
      /     \\     
     | () () |    
      \\  ^  /     
       |||||      
      /|   |\\     
  `;

  const fastfetchOutput = `
<span class="ascii-art">
   .-------------.     <span class="info-key">user</span>@<span class="info-key">wired</span>
  /  _____ _____  \\    ------------------
 |  /  _  \\  _  \\  |   <span class="info-key">OS:</span> Debian GNU/Linux 13 (trixie) x86_64
 | |  / \\  / \\  | |  <span class="info-key">Host:</span> Custom Hardware Workspace
 | | |   ||   | | |  <span class="info-key">Kernel:</span> 6.12.0-custom-x86_64
 |  \\ \\_// \\_//  / |   <span class="info-key">Uptime:</span> 48 hours, 12 mins
  \\  \\___/ \\___/  /    <span class="info-key">Shell:</span> bash 5.2.21
   '-------------'     <span class="info-key">WM:</span> XFCE / LXQt
                       <span class="info-key">Terminal:</span> xterm-256color
                       <span class="info-key">Memory:</span> 4096MiB / 16384MiB

                       <span class="colors-bar">
                         <span style="background:#1e1e1e"></span><span style="background:#484f58"></span><span style="background:#6e7681"></span><span style="background:#8b949e"></span>
                         <span style="background:#c9d1d9"></span><span style="background:#f0f6fc"></span><span style="background:#79c0ff"></span><span style="background:#56d4dd"></span>
                       </span>
</span>`;

  // Автостарт при открытии
  printLine("Initializing Wired System v2.4...");
  printLine("Type '<span class="info-key">help</span>' or '<span class="info-key">fastfetch</span>' to start.\n");

  input.addEventListener('keydown', (e) => {
    if (e.key === 'Enter') {
      const command = input.value.trim();
      printLine(`<span class="prompt">user@wired:~$</span> ${escapeHtml(command)}`);
      processCommand(command.toLowerCase());
      input.value = '';
      window.scrollTo(0, document.body.scrollHeight);
    }
  });

  function processCommand(cmd) {
    switch(cmd) {
      case 'help':
        printLine(`Доступные команды:
  <span class="info-key">fastfetch</span>  - системная информация и арт
  <span class="info-key">whoami</span>     - кто я такой
  <span class="info-key">socials</span>    - ссылки и соцсети
  <span class="info-key">clear</span>      - очистить консоль`);
        break;

      case 'fastfetch':
        printLine(fastfetchOutput);
        break;

      case 'whoami':
        printLine("Студент / Системное администрирование & Python разработчик.");
        break;

      case 'socials':
        printLine("GitHub: https://github.com\nTelegram: @your_tag");
        break;

      case 'clear':
        history.innerHTML = '';
        break;

      case '':
        break;

      default:
        printLine(`bash: command not found: ${escapeHtml(cmd)}. Type 'help' for options.`);
    }
  }

  function printLine(text) {
    const div = document.createElement('div');
    div.className = 'output-line';
    div.innerHTML = text;
    history.appendChild(div);
  }

  function escapeHtml(text) {
    return text.replace(/&/g, "&amp;").replace(/</g, "&lt;").replace(/>/g, "&gt;");
  }
</script>

</body>
</html>
