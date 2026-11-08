  <!-- HEADER -->
  <header>
    <h1>Youtube-theater-curved</h1>
    <p class="tagline">
      Add 20px rounded corners, blended black bars, and a customizable control bar
      to YouTube's theater mode and fullscreen. Now with screenshot, loop, and
      theater-remember tools.
    </p>
    <div class="badges">
      <span class="badge version">v4.1</span>
      <span class="badge manifest">Manifest v3</span>
      <span class="badge license">MIT License</span>
      <span class="badge chrome">Chrome Compatible</span>
    </div>
  </header>

  <!-- SCREENSHOTS -->
  <h2 id="screenshots">📸 Screenshots</h2>
   <div class="screenshot-grid">
    <figure>
      <img src="examples/ytb-theater-md.png" alt="Before theater mode — default YouTube player with square corners and black bars">
    </figure>
  </div>

  <h3>Theater Mode — Before vs After</h3>
  <div class="screenshot-grid">
    <figure>
      <img src="examples/ytb-theater.png" alt="Before theater mode — default YouTube player with square corners and black bars">
    </figure>
  </div>
  
<h3> Theater Mode Light mode </h3>
<div class="screenshot-light">
  <figure>
  <img src="examples/ytb-theater-light.png" alt="After theater mode — rounded corners, blended bars, control bar visible">
  </figure>
</div>

  <h3>Extension Icon</h3>
  <figure style="max-width: 200px;">
    <img src="icons/icon128.png" alt="Extension icon — orange rounded rectangle with play triangle">
  </figure>
  

  <!-- FEATURES -->
  <h2 id="features">✨ Features</h2>

  <h3>🎥 Visual Enhancements</h3>
  <div class="feature-grid">
    <div class="feature-card">
      <h4>20px Rounded Corners</h4>
      <p>Configurable from 5px to 40px via the settings popup, with live preview.</p>
    </div>
    <div class="feature-card">
      <h4>Blended Black Bars</h4>
      <p>Letterbox areas match YouTube's dark/light theme background
      (<code>#0f0f0f</code> / <code>#f9f9f9</code>).</p>
    </div>
    <div class="feature-card">
      <h4>Fullscreen Support</h4>
      <p>Rounded corners and centered video in fullscreen mode.</p>
    </div>
    <div class="feature-card">
      <h4>Light Mode Header Fix</h4>
      <p>The top bar stays light in theater mode — icons, search, logo, and Create button.</p>
    </div>
  </div>

  <h3>🎛️ Custom Control Bar</h3>
  <p>
    A compact, pill-shaped bar that appears <strong>below the player</strong>
    in theater and fullscreen modes, containing:
  </p>

  <table>
    <thead>
      <tr>
        <th>Button</th>
        <th>Action</th>
        <th>Active Color</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>🔁 <strong>Loop</strong></td>
        <td>Repeats the current video</td>
        <td><span style="color: var(--accent); font-weight: 600;">🟠 Orange</span></td>
      </tr>
      <tr>
        <td>📷 <strong>Screenshot</strong></td>
        <td>Saves the current frame as PNG</td>
        <td>—</td>
      </tr>
      <tr>
        <td>🎭 <strong>Theater Remember</strong></td>
        <td>Auto-enters theater mode on every video</td>
        <td><span style="color: var(--accent); font-weight: 600;">🟠 Orange</span></td>
      </tr>
      <tr>
        <td>⚙️ <strong>Settings</strong></td>
        <td>Opens radius slider (5–40px)</td>
        <td>—</td>
      </tr>
    </tbody>
  </table>

  <h3>🧹 Distraction Removal</h3>
  <ul>
    <li>Hides <strong>annotations</strong>, <strong>info cards</strong>, and <strong>card teasers</strong> during theater mode.</li>
  </ul>

  <h3>⚙️ Persistence</h3>
  <ul>
    <li>Settings saved via <code>chrome.storage.sync</code> — sync across all your Chrome devices.</li>
  </ul>

  <h3>🔄 Robust SPA Handling</h3>
  <ul>
    <li>Works when navigating between videos <strong>without refreshing the page</strong>.</li>
    <li>Re-attaches observers automatically after YouTube's internal navigation.</li>
  </ul>

  <!-- INSTALLATION -->
  <h2 id="installation">🚀 Installation</h2>

  <h3>From Source (Developer Mode)</h3>
  <ol>
    <li>
      <strong>Clone the repository</strong>
      <pre><code>git clone https://github.com/your-username/yt-curved.git
cd yt-curved</code></pre>
    </li>
    <li>
      <strong>Open Chrome Extensions</strong>
      <p>Navigate to <code>chrome://extensions/</code> in your browser.</p>
    </li>
    <li>
      <strong>Enable Developer Mode</strong>
      <p>Toggle <strong>Developer mode</strong> in the top-right corner.</p>
    </li>
    <li>
      <strong>Load Unpacked</strong>
      <p>Click <strong>Load unpacked</strong> and select the <code>yt-curved</code> folder.</p>
    </li>
    <li>
      <strong>Done!</strong>
      <p>The orange play-button icon will appear in your toolbar.</p>
    </li>
  </ol>

  <h3>From Chrome Web Store</h3>
  <p><em>Coming soon — link will be added once published.</em></p>

  <!-- USAGE -->
  <h2 id="usage">🖱️ Usage</h2>

  <ol>
    <li>Open any YouTube video at <code>youtube.com/watch?v=...</code>.</li>
    <li>Press <kbd>T</kbd> (or click the theater mode button) to enter theater mode.</li>
    <li>The video gets <strong>rounded corners</strong> and the <strong>custom bar appears below the player</strong>.</li>
    <li>Click the buttons in the bar:
      <ul>
        <li>🔁 <strong>Loop</strong> — toggles video looping.</li>
        <li>📷 <strong>Camera</strong> — downloads a PNG of the current frame.</li>
        <li>🎭 <strong>Theater icon</strong> — enables auto-theater mode on future videos.</li>
        <li>⚙️ <strong>Settings</strong> — opens the radius slider.</li>
      </ul>
    </li>
    <li>Press <kbd>F</kbd> to go fullscreen — corners stay rounded.</li>
    <li>Press <kbd>T</kbd> again to exit theater mode.</li>
  </ol>

  <!-- SETTINGS -->
  <h2 id="settings">⚙️ Settings</h2>

  <p>The settings popup appears when you click the ⚙️ icon in the control bar.</p>

  <table>
    <thead>
      <tr>
        <th>Setting</th>
        <th>Range</th>
        <th>Default</th>
        <th>Description</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td><strong>Radius</strong></td>
        <td>5–40 px</td>
        <td>20 px</td>
        <td>Corner rounding of the video</td>
      </tr>
      <tr>
        <td><strong>Remember Theater</strong></td>
        <td>on / off</td>
        <td>off</td>
        <td>Auto-enter theater mode on every video</td>
      </tr>
    </tbody>
  </table>

  <p>All settings are stored in <code>chrome.storage.sync</code> and persist across sessions.</p>

  <!-- TECHNICAL -->
  <h2 id="technical">🛠️ Technical Details</h2>

  <h3>How It Works</h3>
  <p>
    The extension adds two CSS classes to the <code>&lt;html&gt;</code> element based on
    YouTube's player state:
  </p>

  <table>
    <thead>
      <tr>
        <th>Class</th>
        <th>When Applied</th>
        <th>Effect</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td><code>yt-theater-curved</code></td>
        <td>Theater mode is active</td>
        <td>Rounds video, blends bars, shows control bar</td>
      </tr>
      <tr>
        <td><code>yt-fullscreen-curved</code></td>
        <td>Fullscreen is active</td>
        <td>Rounds video, centers it with symmetric letterboxing</td>
      </tr>
    </tbody>
  </table>

  <h3>Detection Methods (Fallback Chain)</h3>
  <ol>
    <li>Theater button's <code>aria-pressed="true"</code> attribute.</li>
    <li><code>ytd-watch-flexy[theater]</code> attribute.</li>
    <li><code>document.body.classList.contains('theater')</code>.</li>
    <li>Fullscreen API + <code>#movie_player.ytp-fullscreen</code> class.</li>
  </ol>

  <h3>Key CSS Variables</h3>
  <pre><code>:root {
  --yt-curved-radius: 20px;      /* Corner radius, updated by JS */
  --yt-curved-orange: #ff7a00;   /* Active button color */
}</code></pre>

  <h3>Permissions</h3>
  <table>
    <thead>
      <tr>
        <th>Permission</th>
        <th>Reason</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td><code>storage</code></td>
        <td>Save user settings (radius, remember-theater) across sessions</td>
      </tr>
    </tbody>
  </table>


  <!-- ROADMAP -->
  <h2 id="roadmap">🗺️ Roadmap</h2>

  <ul style="list-style: none; padding-left: 0;">
    <li>✅ Rounded corners on video (theater + fullscreen)</li>
    <li>✅ Blended black bars (dark/light theme)</li>
    <li>✅ Custom control bar with buttons</li>
    <li>✅ Configurable radius (5–40px)</li>
    <li>✅ Loop button</li>
    <li>✅ Screenshot button</li>
    <li>✅ Remember theater mode</li>
    <li>✅ Header fix for light mode</li>
  </ul>


  <!-- SUPPORT -->
  <h2 id="support">⭐ Show Your Support</h2>

  <p>If you find this extension useful, please:</p>

  <ul>
    <li>⭐ <strong>Star</strong> the repository</li>
    <li>🐛 <strong>Report</strong> bugs</li>
    <li>💡 <strong>Suggest</strong> features</li>
    <li>📢 <strong>Share</strong> with friends</li>
  </ul>

  <!-- FOOTER -->
  <footer>
    <p>Made with <span class="heart">❤</span> for YouTube lovers</p>
    <a class="back-to-top" href="#screenshots">⬆ Back to top</a>
  </footer>

</div>

</body>
</html>
