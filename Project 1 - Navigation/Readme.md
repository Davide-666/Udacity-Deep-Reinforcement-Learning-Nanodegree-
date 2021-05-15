<!DOCTYPE html>
<html lang="en" data-color-mode="auto" data-light-theme="light" data-dark-theme="dark">
<body>
<h3>The project</h3>
<p>For this project, you will train an agent to navigate (and collect bananas!) in a large, square world.</p>
<p><a target="_blank" rel="noopener noreferrer" href="https://user-images.githubusercontent.com/10624937/42135619-d90f2f28-7d12-11e8-8823-82b970a54d7e.gif"><img src="https://user-images.githubusercontent.com/10624937/42135619-d90f2f28-7d12-11e8-8823-82b970a54d7e.gif" alt="Trained Agent" title="Trained Agent" style="max-width:100%;"></a></p>
<p>A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana.  Thus, the goal of your agent is to collect as many yellow bananas as possible while avoiding blue bananas.</p>
<p>The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around agent's forward direction.  Given this information, the agent has to learn how to best select actions.  Four discrete actions are available, corresponding to:</p>
<ul>
<li><strong><code>0</code></strong> - move forward.</li>
<li><strong><code>1</code></strong> - move backward.</li>
<li><strong><code>2</code></strong> - turn left.</li>
<li><strong><code>3</code></strong> - turn right.</li>
</ul>
<p>The task is episodic, and in order to solve the environment, your agent must get an average score of +13 over 100 consecutive episodes.</p>
<h3><a id="user-content-getting-started" class="anchor" aria-hidden="true" href="#getting-started"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Getting Started</h3>
<ol>
<li>
<p>Download the environment from one of the links below.  You need only select the environment that matches your operating system:</p>
<ul>
<li>Linux: <a href="https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip" rel="nofollow">click here</a></li>
<li>Mac OSX: <a href="https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip" rel="nofollow">click here</a></li>
<li>Windows (32-bit): <a href="https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip" rel="nofollow">click here</a></li>
<li>Windows (64-bit): <a href="https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip" rel="nofollow">click here</a></li>
</ul>
<p>(<em>For Windows users</em>) Check out <a href="https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64" rel="nofollow">this link</a> if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.</p>
<p>(<em>For AWS</em>) If you'd like to train the agent on AWS (and have not <a href="https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md">enabled a virtual screen</a>), then please use <a href="https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux_NoVis.zip" rel="nofollow">this link</a> to obtain the environment.</p>
</li>
<li>
<p>Place the file in the DRLND GitHub repository, in the <code>p1_navigation/</code> folder, and unzip (or decompress) the file.</p>
</li>
</ol>
<h3>Instructions</h3>
 <p> The main application is the notebook Navigation-application&report.ipynb </p>
 <p> The algorithm implements a Deep Q-Network (DQN) to approximate the Q-function </p>
 <p> The main application is the notebook Navigation-application&report.ipynb </p>
 <p> The main application is the notebook Navigation-application&report.ipynb </p>
 
<h3>What's next: 1) Implement Dueling and Double Deep Q-Network (DDQN) </h3>
<h3>What's next: 2) Challenge: Learning from Pixels</h3>
<p>After you have successfully completed the project, if you're looking for an additional challenge, you have come to the right place!  In the project, your agent learned from information such as its velocity, along with ray-based perception of objects around its forward direction.  A more challenging task would be to learn directly from pixels!</p>
<p>To solve this harder task, you'll need to download a new Unity environment.  This environment is almost identical to the project environment, where the only difference is that the state is an 84 x 84 RGB image, corresponding to the agent's first-person view.  (<strong>Note</strong>: Udacity students should not submit a project with this new environment.)</p>
<p>You need only select the environment that matches your operating system:</p>
<ul>
<li>Linux: <a href="https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/VisualBanana_Linux.zip" rel="nofollow">click here</a></li>
<li>Mac OSX: <a href="https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/VisualBanana.app.zip" rel="nofollow">click here</a></li>
<li>Windows (32-bit): <a href="https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/VisualBanana_Windows_x86.zip" rel="nofollow">click here</a></li>
<li>Windows (64-bit): <a href="https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/VisualBanana_Windows_x86_64.zip" rel="nofollow">click here</a></li>
</ul>
<p>Then, place the file in the <code>p1_navigation/</code> folder in the DRLND GitHub repository, and unzip (or decompress) the file.  Next, open <code>Navigation_Pixels.ipynb</code> and follow the instructions to learn how to use the Python API to control the agent.</p>
<p>(<em>For AWS</em>) If you'd like to train the agent on AWS, you must follow the instructions to <a href="https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md">set up X Server</a>, and then download the environment for the <strong>Linux</strong> operating system above.</p>
</article>
  </div>  
  </body>
</html>
