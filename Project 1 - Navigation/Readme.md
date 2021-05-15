<!DOCTYPE html>
<html lang="en" data-color-mode="auto" data-light-theme="light" data-dark-theme="dark">
<body>
<h3>The project</h3>
<p>For this project, an agent is trined to navigate (and collect bananas!) in a large, square world.</p>
<p><a target="_blank" rel="noopener noreferrer" href="https://user-images.githubusercontent.com/10624937/42135619-d90f2f28-7d12-11e8-8823-82b970a54d7e.gif"><img src="https://user-images.githubusercontent.com/10624937/42135619-d90f2f28-7d12-11e8-8823-82b970a54d7e.gif" alt="Trained Agent" title="Trained Agent" style="max-width:100%;"></a></p>
<p>A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana.  Thus, the goal of the agent is to collect as many yellow bananas as possible while avoiding blue bananas.</p>
<p>The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around agent's forward direction.  Given this information, the agent has to learn how to best select actions.  Four discrete actions are available, corresponding to:</p>
<ul>
<li><strong><code>0</code></strong> - move forward.</li>
<li><strong><code>1</code></strong> - move backward.</li>
<li><strong><code>2</code></strong> - turn left.</li>
<li><strong><code>3</code></strong> - turn right.</li>
</ul>
<p>The task is episodic, and in order to solve the environment, the agent must get an average score of +13 over 100 consecutive episodes.</p>
<h3>Getting Started</h3>
<ol>
<li>
<p>If you want to run the application locally, you need to download the environment from one of the links below.  You need only select the environment that matches your operating system:</p>
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
 <p> The main application is the notebook Navigation-application&report.ipynb where the agent is trained and tested.</p>
 <p> The "main" algorithm implements a Deep Q-Network (DQN) to approximate the Q-function </p>
 <p> The application implements the following steps: </p>
 <p> 1) Import the Necessary Packages (including the support funcions contained in the files model.py and dqn_agent.py from the Deep Q-Network exercise <br>
     2) Examine the State and Action Spaces <br>
     3) Train an agent using DQN <br>
     4) Plot the scores <br>
 </p>
<h3>Hyperparamenter</h3>
<p> BUFFER_SIZE = int(1e5)  # replay buffer size <br>
BATCH_SIZE = 64         # minibatch size <br>
GAMMA = 0.99            # discount factor <br>
TAU = 1e-3              # for soft update of target parameters <br>
LR = 5e-4               # learning rate  <br>
UPDATE_EVERY = 4        # how often to update the network <br></p>
 
 <h3>DQN structure</h3>
<p> DQN has the following structure: <br>
1 - Fully collected layer, input dim 37, output dim 128. RELU activation <br>
2 - Fully collected layer, input dim 128, output dim 64. RELU activation <br>
3 - Fully collected layer, input dim 64, output dim 4 <br>
 <br>
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
  <p> You can read more about ML-Agents by perusing the GitHub repository (https://github.com/Unity-Technologies/ml-agents). The project environment is similar to, but not identical to the Banana Collector environment on the Unity ML-Agents GitHub page (https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#banana-collector)</p>

  
  </body>
</html>
