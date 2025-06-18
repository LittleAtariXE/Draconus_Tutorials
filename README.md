<h1 align="center">🐉 Draconus Tutorials</h1>
  <p align="center">
    This repository contains tutorials and guides for using the <strong>Draconus</strong> project.<br>
    You'll find videos and instructions covering installation, running the system, building worms, and more.
  </p>
<hr>
<h2>📹 Tutorial 1: Installing Draconus, Docker, and Adding User to Group</h2>
  <p>
    This first video tutorial walks you through the setup process:
  </p>
  <ul>
    <li>Installing <strong>Docker</strong> on your system: <code>sudo apt install docker.io</code></li>
    <li>Adding your user to the <code>sudo usermod -aG docker $USER</code> group</li>
    <li>Reboot or relogin system</li>
  </ul>
  <p>
    ▶️ <a href="https://vimeo.com/1094387484/8c8582b2f0" target="_blank">
      Watch on Vimeo
    </a>
  </p>
  <hr>
<h2>📹 Tutorial 2: Properly Launching Draconus</h2>
  <p>
    This tutorial explains how to correctly start the <strong>Draconus</strong> system using two terminal windows.
  </p>
  <ul>
    <li>Navigate to the <code>Draconus</code> project directory.</li>
    <li>Open <strong>two terminal windows</strong>.</li>
    <li>In the <strong>first terminal</strong>, run:<br>
      <code>python3 Draconus.py</code><br>
      This will start the main <strong>Draconus</strong> background service.<br>
      You can run it in the background using tools like <code>nohup</code> if desired.
    </li>
    <li>In the <strong>second terminal</strong>, run:<br>
      <code>python3 c2.py</code><br>
      This will start the <strong>Commander</strong> interface.<br>
      On the first run, it will automatically create a <code>venv</code> environment and install all necessary dependencies.
    </li>
  </ul>
  <p>
    ⚠️ <strong>Important!</strong><br>
    The <code>exit</code> command only closes the Commander interface — <strong>Draconus will keep running in the background</strong>.<br>
    Use the <code>quit</code> command to properly shut down both programs.
  </p>
  <p>
    ▶️ <a href="https://vimeo.com/1094410166/c754f7a280" target="_blank">
      Watch Tutorial 2 on Vimeo
    </a>
  </p>
<hr>
<h2>📹 Tutorial 3: Building and Installing the Compiler</h2>

<p>
  This tutorial explains how to install the cross-compilation system used by <strong>Draconus</strong> for building Windows executables directly from Linux.
</p>

<ul>
  <li>Go to the <code>hive</code> section inside the Commander interface.</li>
  <li>Type the command:<br>
    <code>install</code><br>
    This will show a list of available compilers along with their name, image size, availability, and description.
  </li>
  <li>If the desired compiler (e.g., <code>CrossComp</code>) is not yet installed, run:<br>
    <code>install -i CrossComp</code><br>
    This command will start downloading the required Docker image and begin building the compiler environment. It may take several minutes.
  </li>
  <li>
    The compiler setup will take approximately <strong>5.5 GB</strong> of additional disk space.<br>
    This includes the entire Linux-based system, emulators, and Windows cross-compilation toolchains.
  </li>
  <li>
    Once the compiler is built, exit and re-enter the <code>hive</code> section to refresh the environment and apply the changes.
  </li>
  <li>
    ✅ You are now ready to build <code>.exe</code> files directly from Linux!
  </li>
</ul>

<p>
  ▶️ <a href="https://vimeo.com/1094444812/645fe7987d" target="_blank">
    Watch Tutorial 3 on Vimeo
  </a>
</p>

  
<hr>
<h3>📁 More tutorials coming soon...</h3>
<p>
  Stay tuned for future videos on:
</p>
<ul>
  <li>Using Draconus server types</li>
  <li>Creating and managing worms</li>
</ul>
