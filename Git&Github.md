# <p style="color:#33B3DE; text-align:center;">**GIT**</p>

<p style="font-size:18px;">Git is the free and open source distributed version control system designed to handle everything from small to large scale projects with speed and efficiency.</p>

# <p style="color:#33B3DE; text-align:center;">**GITHUB**</p>

<p style="font-size:18px;">Github is the intenet hosting service for software development and version control using Git. or in other words github is a website that uses git to keep a track and save your work progress in Repositories/(Directories or Folders) just like a cloud space.</p>

---

## <p style="color:#33B3DE; text-align:center;">**SSH Keys**</p>

<p style="font-size:20px;">An SSH key is an access credential for the SSH (secure shell) network protocol.<br/>
This authenticated and encrypted secure network protocol is used for remote communication between machines on an unsecured open network.<br/>
SSH keys are generated through a public key cryptographic algorithm, the most common being RSA or DSA.<br/>
At a very high level SSH keys are generated through a mathematical formula that takes 2 prime numbers and a random seed variable to output the public and private key. This is a one-way formula that ensures the public key can be derived from the private key but the private key cannot be derived from the public key.</p>

## <p style="color:#3CD041;">1. execute the following to begin the key creation

> <p style="font-size:22px;">ssh-keygen -t rsa -b 4096 -C "your_email@example.com"</p>

<p style="font-size:18px;">This command will create a new SSH key using the email as a label</p>

## <p style="color:#3CD041;">2. You will then be prompted to "Enter a file in which to save the key."<br/>You can specify a file location or press “Enter” to accept the default file location.</p>

> <p style="font-size:22px;">Enter a file in which to save the key (/Users/you/.ssh/id_rsa): [Press enter]</p>

## <p style="color:#3CD041;">3. The next prompt will ask for a secure passphrase.</p>

<p style="font-size:18px;">A passphrase will add an additional layer of security to the SSH and will be required anytime the SSH key is used. If someone gains access to the computer that private keys are stored on, they could also gain access to any system that uses that key. Adding a passphrase to keys will prevent this scenario.</p>

> <p style="font-size:22px;">Enter passphrase (empty for no passphrase): [Type a passphrase]<br/>Enter same passphrase again: [Type passphrase again]</p>

<p style="font-size:18px">At this point, a new SSH key will have been generated at the previously specified file path.</p>

## <p style="color:#3CD041;">4. Adding your SSH key to the ssh-agent</p>

<p style="font-size:20px">Before adding a new SSH key to the ssh-agent to manage your keys, you should have checked for existing SSH keys and generated a new SSH key.</p>
<p style="font-size:18px">(a). Ensure the ssh-agent is running.</p>

> <p style="font-size:22px;">eval "$(ssh-agent -s)<br/>Agent pid 59566</p>

<p style="font-size:18px">(b). Add your SSH private key to the ssh-agent. If you created your key with a different name, or if you are adding an existing key that has a different name, replace id_ed25519 in the command with the name of your private key file.</p>

> <p style="font-size:22px;">ssh-add ~/.ssh/id_ed25519</p>

## <p style="color:#3CD041;">5. Add the SSH key to your account on GitHub</p>

<p style="font-size:18px">(a). Copy the SSH public key to your clipboard.</p>

> <p style="font-size:22px;">clip < ~/.ssh/id_ed25519.pub<br/># Copies the contents of the id_ed25519.pub file to your clipboard</p>
> <p style="font-size:16px; font-weight:400; color:white">Tip: If clip isn't working, you can locate the hidden .ssh folder, open the file in your favorite text editor, and copy it to your clipboard</p><br/>

<p style="font-size:18px;">(b). In the upper-right corner of any page, click your profile photo, then click <strong>Settings</strong>.</p>

![Github add ssh settings](MDimages/userbar-account-settings.png)

<p style="font-size:18px">(c). In the "Access" section of the sidebar, click  <strong>SSH and GPG keys</strong>.</p>
